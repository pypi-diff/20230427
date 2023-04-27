# Comparing `tmp/revup-0.2.0.tar.gz` & `tmp/revup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revup-0.2.0.tar", last modified: Tue Apr 25 18:54:51 2023, max compression
+gzip compressed data, was "revup-0.2.1.tar", last modified: Thu Apr 27 21:06:02 2023, max compression
```

## Comparing `revup-0.2.0.tar` & `revup-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.117042 revup-0.2.0/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1069 2023-01-11 23:02:09.000000 revup-0.2.0/LICENSE
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    12928 2023-04-25 18:54:51.117042 revup-0.2.0/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    11281 2023-01-11 23:02:09.000000 revup-0.2.0/README.md
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:02:09.000000 revup-0.2.0/pyproject.toml
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.113042 revup-0.2.0/revup/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      147 2023-04-25 18:52:57.000000 revup-0.2.0/revup/__init__.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      976 2023-04-15 00:51:58.000000 revup-0.2.0/revup/__main__.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     9280 2023-04-13 20:59:39.000000 revup-0.2.0/revup/amend.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2653 2023-04-13 20:59:39.000000 revup-0.2.0/revup/cherry_pick.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3568 2023-04-13 17:46:12.000000 revup-0.2.0/revup/config.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    29863 2023-04-14 21:18:39.000000 revup-0.2.0/revup/git.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      394 2023-01-11 23:02:09.000000 revup-0.2.0/revup/github.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2817 2023-01-11 23:02:09.000000 revup-0.2.0/revup/github_real.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    21678 2023-04-15 00:51:58.000000 revup-0.2.0/revup/github_utils.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2302 2023-04-13 20:59:39.000000 revup-0.2.0/revup/logs.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.113042 revup-0.2.0/revup/man1/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1336 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/amend.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      692 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/cherry-pick.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1019 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/config.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      931 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/restack.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2194 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/revup.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3492 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/upload.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      412 2023-04-13 20:59:39.000000 revup-0.2.0/revup/restack.py
--rwxrwxr-x   0 jerry     (1000) jerry     (1000)    16057 2023-04-13 17:46:12.000000 revup-0.2.0/revup/revup.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     9819 2023-01-11 23:02:09.000000 revup-0.2.0/revup/shell.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2402 2023-03-06 21:56:06.000000 revup-0.2.0/revup/toolkit.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    63501 2023-04-14 01:18:56.000000 revup-0.2.0/revup/topic_stack.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2490 2023-04-19 02:22:49.000000 revup-0.2.0/revup/types.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3652 2023-04-13 23:09:23.000000 revup-0.2.0/revup/upload.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.113042 revup-0.2.0/revup.egg-info/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    12928 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      725 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/SOURCES.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/dependency_links.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       47 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/entry_points.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       85 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/requires.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        6 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/top_level.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1817 2023-04-25 18:54:51.117042 revup-0.2.0/setup.cfg
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      861 2023-01-11 23:02:09.000000 revup-0.2.0/setup.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.117042 revup-0.2.0/tests/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1569 2023-01-11 23:02:09.000000 revup-0.2.0/tests/test_tools.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-27 21:06:02.411223 revup-0.2.1/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1069 2023-01-11 23:02:09.000000 revup-0.2.1/LICENSE
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    12995 2023-04-27 21:06:02.411223 revup-0.2.1/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    11348 2023-04-25 19:04:39.000000 revup-0.2.1/README.md
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:02:09.000000 revup-0.2.1/pyproject.toml
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-27 21:06:02.411223 revup-0.2.1/revup/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      147 2023-04-27 21:05:18.000000 revup-0.2.1/revup/__init__.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      976 2023-04-15 00:51:58.000000 revup-0.2.1/revup/__main__.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     9401 2023-04-27 19:54:25.000000 revup-0.2.1/revup/amend.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2653 2023-04-13 20:59:39.000000 revup-0.2.1/revup/cherry_pick.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3568 2023-04-13 17:46:12.000000 revup-0.2.1/revup/config.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    29863 2023-04-14 21:18:39.000000 revup-0.2.1/revup/git.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      394 2023-01-11 23:02:09.000000 revup-0.2.1/revup/github.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2817 2023-01-11 23:02:09.000000 revup-0.2.1/revup/github_real.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    21678 2023-04-15 00:51:58.000000 revup-0.2.1/revup/github_utils.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2302 2023-04-13 20:59:39.000000 revup-0.2.1/revup/logs.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-27 21:06:02.411223 revup-0.2.1/revup/man1/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1335 2023-04-27 21:05:56.000000 revup-0.2.1/revup/man1/amend.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      691 2023-04-27 21:05:56.000000 revup-0.2.1/revup/man1/cherry-pick.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1019 2023-04-27 21:05:56.000000 revup-0.2.1/revup/man1/config.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      929 2023-04-27 21:05:56.000000 revup-0.2.1/revup/man1/restack.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2194 2023-04-27 21:05:56.000000 revup-0.2.1/revup/man1/revup.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3491 2023-04-27 21:05:56.000000 revup-0.2.1/revup/man1/upload.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      412 2023-04-13 20:59:39.000000 revup-0.2.1/revup/restack.py
+-rwxrwxr-x   0 jerry     (1000) jerry     (1000)    16057 2023-04-13 17:46:12.000000 revup-0.2.1/revup/revup.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     9819 2023-01-11 23:02:09.000000 revup-0.2.1/revup/shell.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2402 2023-03-06 21:56:06.000000 revup-0.2.1/revup/toolkit.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    63501 2023-04-14 01:18:56.000000 revup-0.2.1/revup/topic_stack.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2490 2023-04-19 02:22:49.000000 revup-0.2.1/revup/types.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3652 2023-04-13 23:09:23.000000 revup-0.2.1/revup/upload.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-27 21:06:02.411223 revup-0.2.1/revup.egg-info/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    12995 2023-04-27 21:06:02.000000 revup-0.2.1/revup.egg-info/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      725 2023-04-27 21:06:02.000000 revup-0.2.1/revup.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2023-04-27 21:06:02.000000 revup-0.2.1/revup.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       47 2023-04-27 21:06:02.000000 revup-0.2.1/revup.egg-info/entry_points.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       85 2023-04-27 21:06:02.000000 revup-0.2.1/revup.egg-info/requires.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        6 2023-04-27 21:06:02.000000 revup-0.2.1/revup.egg-info/top_level.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1817 2023-04-27 21:06:02.415223 revup-0.2.1/setup.cfg
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      861 2023-01-11 23:02:09.000000 revup-0.2.1/setup.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-27 21:06:02.411223 revup-0.2.1/tests/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1569 2023-01-11 23:02:09.000000 revup-0.2.1/tests/test_tools.py
```

### Comparing `revup-0.2.0/LICENSE` & `revup-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/PKG-INFO` & `revup-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revup
-Version: 0.2.0
+Version: 0.2.1
 Summary: Revolutionary github tools. Effortlessly create multiple branches and pull requests.
 Home-page: https://github.com/skydio/revup
 Author: Jerry Zhang
 Author-email: jerry@skydio.com
 License: MIT
 Project-URL: Source, https://github.com/skydio/revup
 Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
@@ -28,30 +28,30 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
 
-  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/revup_light.svg"/>
+  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/revup_light.svg"/>
 
 </p>
 
 <p align="center">
 <a href="https://github.com/Skydio/revup"><img alt="Source Code" src="https://img.shields.io/badge/source-code-blue"/></a>
 <a href="https://github.com/Skydio/revup/issues"><img alt="Issues" src="https://img.shields.io/badge/issue-tracker-blue"/></a>
 <img alt="Python 3.8 | 3.9 | 3.10" src="https://img.shields.io/pypi/pyversions/revup"/>
 <a href="https://pypi.org/project/revup/"><img alt="PyPI" src="https://img.shields.io/pypi/v/revup"/></a>
 <a href="https://github.com/Skydio/revup/tree/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/pypi/l/revup"/></a>
 </p>
 
 Revup provides command-line tools that allow developers to iterate faster on parallel changes and reduce the overhead of creating and maintaining code reviews.
 
 <p align="center">
-<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif"/>
+<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_1.gif"/>
 </p>
 
 # Features
 
 - Revup creates multiple independent chains of branches for you in the background and without touching your working tree. It then creates and manages github pull requests for all those branches.
 - Pull requests target the actual base branch and can be merged manually or by continuous integration
 - Rebase detection saves time and continuous integration cost by not re-pushing if the patch hasn't changed
@@ -95,19 +95,20 @@
 Clone a sandbox repo by [forking](https://github.com/Skydio/revup/fork) revup, creating a [new](https://github.com/new) repo, or using some other repo you own.
 Creating test PRs can be spammy so don't do the tutorial on other people's repos.
 
 ```sh
 git clone https://github.com/<your-name>/revup.git && cd revup
 ```
 
-On first run, revup will prompt you to add github credentials
+On first run, you will need to configure github credentials. Create a personal access token [here](https://github.com/settings/tokens/new)
+and check the box for "full repo permissions". Revup needs this in order to create and modify pull requests. Then run
 ```sh
-revup upload
+revup config github_oauth
 ```
-Create a personal access token [here](https://github.com/settings/tokens/new) and check the box for "full repo permissions". Revup needs this in order to create and modify pull requests.
+and copy and paste the oauth into the prompt.
 
 ## Create independent pull requests
 
 Make your first two commits that will become two separate pull requests.
 Note the "Topic:" tag in the commit message - this is what causes revup to recognize and act on a commit.
 Each separately named topic will become a new pull request.
 
@@ -116,34 +117,34 @@
 git commit -m "My first revup foo" -m "Topic: foo"
 echo peh > bar; git add bar
 git commit -m "My first revup bar" -m "Topic: bar"
 
 revup upload
 ```
 
-![tutorial_1](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif)
+![tutorial_1](https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_1.gif)
 
 You've uploaded your first revup changes! Notice how in github, both branches target 'main'. This allows them to be merged independently.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/bar_github.png" width="50%">
+<img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/bar_github.png" width="50%">
 
 Under the hood, revup creates and pushes these branches for you, tracking and managing the dependencies as needed.
 
 ## Create relative pull requests
 
 Now we'll make a new review that's relative to "foo". The "Relative" tag will ensure the new review targets the correct branch.
 
 ```sh
 echo deh >> foo; git add foo
 git commit -m "My second revup foo" -m "Topic: foo2" -m "Relative: foo"
 
 revup upload
 ```
 
-![tutorial_2](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif)
+![tutorial_2](https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_2.gif)
 
 With this simple but powerful model, you can upload independent and dependent changes all at once.
 
 - Multiple commits can be in one topic, in which case they will all be in a single pull request.
 - Commits in the same topic do not need to be adjacent in history.
 - Topics relative to each other do not need to be adjacent in history, but the second topic must come after the first.
 
@@ -157,15 +158,15 @@
 revup amend HEAD~ --no-edit  # Specify a commit to amend
 # or
 revup amend bar --no-edit  # Specify a topic name to amend
 
 revup upload
 ```
 
-![tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_3.gif)
+![tutorial_3](https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_3.gif)
 
 `revup amend` makes it easy to modify commits in your history. You also have other options for modifying reviews:
 
 - Adding new commits with the same topic
 - Using `git rebase --interactive` along with `git commit --amend`
 
 ## Pulling in upstream changes
@@ -238,19 +239,19 @@
 revup upload --base-branch custom-branch-name
 ```
 
 ## Review graph and patchsets
 
 Revup will add 2 comments in every pull request to provide helpful features for users and reviewers. These are enabled by default and automatically updated as the pull request changes.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/review_graph.png" width="40%">
+<img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/review_graph.png" width="40%">
 
 The review graph provides links and titles to all local pull requests that have a relative relationship with the current pull request, including any that it depends on, or that depend on it. This allows you to quickly browse between pull requests in a chain.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png" width="80%">
+<img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/patchsets.png" width="80%">
 
 The patchsets table provides a history of uploads for a given pull request as well as links and summaries of the diff between each upload. Notably, revup specially handles
 the case where you rebase then upload and will show you a diff with upstream files excluded.
 
 # Configuring revup
 
 Revup is highly configurable using a standard config file format. Every flag is also a config option, so users can get the exact behavior they need.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revup Version: 0.2.0 Summary: Revolutionary github
+Metadata-Version: 2.1 Name: revup Version: 0.2.1 Summary: Revolutionary github
 tools. Effortlessly create multiple branches and pull requests. Home-page:
 https://github.com/skydio/revup Author: Jerry Zhang Author-email:
 jerry@skydio.com License: MIT Project-URL: Source, https://github.com/skydio/
 revup Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
 Keywords: github python git workflow version-control python3 developer-tools
 code-review pull-requests developers developer-productivity stacked-diffs
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -41,45 +41,46 @@
 can also build from source to get the latest updates. ``` git clone https://
 github.com/Skydio/revup.git && cd revup make deps && make package && make
 install ``` # Tutorial This tutorial will guide you through using basic revup
 features. ## First time setup Clone a sandbox repo by [forking](https://
 github.com/Skydio/revup/fork) revup, creating a [new](https://github.com/new)
 repo, or using some other repo you own. Creating test PRs can be spammy so
 don't do the tutorial on other people's repos. ```sh git clone https://
-github.com//revup.git && cd revup ``` On first run, revup will prompt you to
-add github credentials ```sh revup upload ``` Create a personal access token
-[here](https://github.com/settings/tokens/new) and check the box for "full repo
-permissions". Revup needs this in order to create and modify pull requests. ##
-Create independent pull requests Make your first two commits that will become
-two separate pull requests. Note the "Topic:" tag in the commit message - this
-is what causes revup to recognize and act on a commit. Each separately named
-topic will become a new pull request. ```sh echo meh > foo; git add foo git
-commit -m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git
-commit -m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1]
-(https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
-tutorial_1.gif) You've uploaded your first revup changes! Notice how in github,
-both branches target 'main'. This allows them to be merged independently.
-[https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
-foo_github.png][https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
-images/bar_github.png] Under the hood, revup creates and pushes these branches
-for you, tracking and managing the dependencies as needed. ## Create relative
-pull requests Now we'll make a new review that's relative to "foo". The
-"Relative" tag will ensure the new review targets the correct branch. ```sh
-echo deh >> foo; git add foo git commit -m "My second revup foo" -m "Topic:
-foo2" -m "Relative: foo" revup upload ``` ![tutorial_2](https://
-raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif) With
+github.com//revup.git && cd revup ``` On first run, you will need to configure
+github credentials. Create a personal access token [here](https://github.com/
+settings/tokens/new) and check the box for "full repo permissions". Revup needs
+this in order to create and modify pull requests. Then run ```sh revup config
+github_oauth ``` and copy and paste the oauth into the prompt. ## Create
+independent pull requests Make your first two commits that will become two
+separate pull requests. Note the "Topic:" tag in the commit message - this is
+what causes revup to recognize and act on a commit. Each separately named topic
+will become a new pull request. ```sh echo meh > foo; git add foo git commit -
+m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git commit -
+m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1](https://
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_1.gif)
+You've uploaded your first revup changes! Notice how in github, both branches
+target 'main'. This allows them to be merged independently. [https://
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/foo_github.png]
+[https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/
+bar_github.png] Under the hood, revup creates and pushes these branches for
+you, tracking and managing the dependencies as needed. ## Create relative pull
+requests Now we'll make a new review that's relative to "foo". The "Relative"
+tag will ensure the new review targets the correct branch. ```sh echo deh >>
+foo; git add foo git commit -m "My second revup foo" -m "Topic: foo2" -
+m "Relative: foo" revup upload ``` ![tutorial_2](https://
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_2.gif) With
 this simple but powerful model, you can upload independent and dependent
 changes all at once. - Multiple commits can be in one topic, in which case they
 will all be in a single pull request. - Commits in the same topic do not need
 to be adjacent in history. - Topics relative to each other do not need to be
 adjacent in history, but the second topic must come after the first. ## Modify
 pull requests Now let's update a pull request. ```sh echo heh >> bar; git add
 bar # Either revup amend HEAD~ --no-edit # Specify a commit to amend # or revup
 amend bar --no-edit # Specify a topic name to amend revup upload ``` !
-[tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
+[tutorial_3](https://raw.githubusercontent.com/skydio/revup/917438e/docs/
 images/tutorial_3.gif) `revup amend` makes it easy to modify commits in your
 history. You also have other options for modifying reviews: - Adding new
 commits with the same topic - Using `git rebase --interactive` along with `git
 commit --amend` ## Pulling in upstream changes Use `git pull --rebase` to pull
 in changes. Don't use `git merge` or `git pull` without rebase as this creates
 a merge commit. By default revup will not upload if you pull but haven't made
 changes to a commit. To override this and upload always, run `revup upload --
@@ -110,20 +111,20 @@
 latter case). ``` A fix for multiple branches Topic: fix Branches: main, rel1.1
 ``` You can specify base branch on the command line as well, although this is
 usually not necessary unless you're working on a branch that the autodetector
 doesn't know about (see Repo config below). ``` revup upload --base-branch
 custom-branch-name ``` ## Review graph and patchsets Revup will add 2 comments
 in every pull request to provide helpful features for users and reviewers.
 These are enabled by default and automatically updated as the pull request
-changes. [https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
+changes. [https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/
 review_graph.png] The review graph provides links and titles to all local pull
 requests that have a relative relationship with the current pull request,
 including any that it depends on, or that depend on it. This allows you to
 quickly browse between pull requests in a chain. [https://
-raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png] The
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/patchsets.png] The
 patchsets table provides a history of uploads for a given pull request as well
 as links and summaries of the diff between each upload. Notably, revup
 specially handles the case where you rebase then upload and will show you a
 diff with upstream files excluded. # Configuring revup Revup is highly
 configurable using a standard config file format. Every flag is also a config
 option, so users can get the exact behavior they need. Flags specified on the
 command line take precedence, followed by config in `~/.revupconfig`, followed
```

### Comparing `revup-0.2.0/README.md` & `revup-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -69,19 +69,20 @@
 Clone a sandbox repo by [forking](https://github.com/Skydio/revup/fork) revup, creating a [new](https://github.com/new) repo, or using some other repo you own.
 Creating test PRs can be spammy so don't do the tutorial on other people's repos.
 
 ```sh
 git clone https://github.com/<your-name>/revup.git && cd revup
 ```
 
-On first run, revup will prompt you to add github credentials
+On first run, you will need to configure github credentials. Create a personal access token [here](https://github.com/settings/tokens/new)
+and check the box for "full repo permissions". Revup needs this in order to create and modify pull requests. Then run
 ```sh
-revup upload
+revup config github_oauth
 ```
-Create a personal access token [here](https://github.com/settings/tokens/new) and check the box for "full repo permissions". Revup needs this in order to create and modify pull requests.
+and copy and paste the oauth into the prompt.
 
 ## Create independent pull requests
 
 Make your first two commits that will become two separate pull requests.
 Note the "Topic:" tag in the commit message - this is what causes revup to recognize and act on a commit.
 Each separately named topic will become a new pull request.
```

#### html2text {}

```diff
@@ -22,26 +22,27 @@
 can also build from source to get the latest updates. ``` git clone https://
 github.com/Skydio/revup.git && cd revup make deps && make package && make
 install ``` # Tutorial This tutorial will guide you through using basic revup
 features. ## First time setup Clone a sandbox repo by [forking](https://
 github.com/Skydio/revup/fork) revup, creating a [new](https://github.com/new)
 repo, or using some other repo you own. Creating test PRs can be spammy so
 don't do the tutorial on other people's repos. ```sh git clone https://
-github.com//revup.git && cd revup ``` On first run, revup will prompt you to
-add github credentials ```sh revup upload ``` Create a personal access token
-[here](https://github.com/settings/tokens/new) and check the box for "full repo
-permissions". Revup needs this in order to create and modify pull requests. ##
-Create independent pull requests Make your first two commits that will become
-two separate pull requests. Note the "Topic:" tag in the commit message - this
-is what causes revup to recognize and act on a commit. Each separately named
-topic will become a new pull request. ```sh echo meh > foo; git add foo git
-commit -m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git
-commit -m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1]
-(docs/images/tutorial_1.gif) You've uploaded your first revup changes! Notice
-how in github, both branches target 'main'. This allows them to be merged
+github.com//revup.git && cd revup ``` On first run, you will need to configure
+github credentials. Create a personal access token [here](https://github.com/
+settings/tokens/new) and check the box for "full repo permissions". Revup needs
+this in order to create and modify pull requests. Then run ```sh revup config
+github_oauth ``` and copy and paste the oauth into the prompt. ## Create
+independent pull requests Make your first two commits that will become two
+separate pull requests. Note the "Topic:" tag in the commit message - this is
+what causes revup to recognize and act on a commit. Each separately named topic
+will become a new pull request. ```sh echo meh > foo; git add foo git commit -
+m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git commit -
+m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1](docs/
+images/tutorial_1.gif) You've uploaded your first revup changes! Notice how in
+github, both branches target 'main'. This allows them to be merged
 independently. [docs/images/foo_github.png][docs/images/bar_github.png] Under
 the hood, revup creates and pushes these branches for you, tracking and
 managing the dependencies as needed. ## Create relative pull requests Now we'll
 make a new review that's relative to "foo". The "Relative" tag will ensure the
 new review targets the correct branch. ```sh echo deh >> foo; git add foo git
 commit -m "My second revup foo" -m "Topic: foo2" -m "Relative: foo" revup
 upload ``` ![tutorial_2](docs/images/tutorial_2.gif) With this simple but
```

### Comparing `revup-0.2.0/revup/__main__.py` & `revup-0.2.1/revup/__main__.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/amend.py` & `revup-0.2.1/revup/amend.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,27 +190,27 @@
         if stack[0].commit_msg == new_msg and not has_diff:
             return 0
 
         stack[0].commit_msg = new_msg
 
     if has_diff:
         new_commit = stack[0].parents[0]
-
+        if not args.drop:
+            stack[-1].tree = GitTreeHash(await git_ctx.git_stdout("write-tree"))
         for i, commit_obj in enumerate(stack):
             if i == 0 and args.drop:
                 # Drop the target commit
                 continue
             elif i == 0 and len(stack) > 1:
                 # Perform an amend for the first commit, unless there's only one
                 # in which case we can use the tree shortcut.
-                temp_commit = CommitHeader(
-                    GitTreeHash(await git_ctx.git_stdout("write-tree")), [git.HEAD_COMMIT]
-                )
+                temp_commit = CommitHeader(stack[-1].tree, [git.HEAD_COMMIT])
                 temp_commit.title = temp_commit.commit_msg = "cached changes"
                 temp_commit.commit_id = await git_ctx.commit_tree(temp_commit)
+                # drop must be false, so this will be the result of write-tree from above
                 stack[-1].tree = temp_commit.tree
                 try:
                     new_commit = await git_ctx.synthetic_amend(commit_obj, temp_commit)
                 except GitConflictException as exc:
                     await git_ctx.dump_conflict(exc)
                     raise RevupConflictException(
                         temp_commit,
```

### Comparing `revup-0.2.0/revup/cherry_pick.py` & `revup-0.2.1/revup/cherry_pick.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/config.py` & `revup-0.2.1/revup/config.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/git.py` & `revup-0.2.1/revup/git.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/github_real.py` & `revup-0.2.1/revup/github_real.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/github_utils.py` & `revup-0.2.1/revup/github_utils.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/logs.py` & `revup-0.2.1/revup/logs.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/man1/revup.1.gz` & `revup-0.2.1/revup/man1/revup.1.gz`

 * *Files 4% similar despite different names*

#### revup.1

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 1.19.2.4
 .\"
-.TH "revup" "1" "Apr 21, 2021" "revup 0.2.0" "Revup Manual"
+.TH "revup" "1" "Apr 21, 2021" "revup 0.2.1" "Revup Manual"
 .hy
 .SH NAME
 .PP
 revup \- Efficient git workflow and code review toolkit
 .SH SYNOPSIS
 .PP
 \f[C]revup\ [<options>]\ <command>\ [<args>]\f[]
```

### Comparing `revup-0.2.0/revup/revup.py` & `revup-0.2.1/revup/revup.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/shell.py` & `revup-0.2.1/revup/shell.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/toolkit.py` & `revup-0.2.1/revup/toolkit.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/topic_stack.py` & `revup-0.2.1/revup/topic_stack.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/types.py` & `revup-0.2.1/revup/types.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup/upload.py` & `revup-0.2.1/revup/upload.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/revup.egg-info/PKG-INFO` & `revup-0.2.1/revup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revup
-Version: 0.2.0
+Version: 0.2.1
 Summary: Revolutionary github tools. Effortlessly create multiple branches and pull requests.
 Home-page: https://github.com/skydio/revup
 Author: Jerry Zhang
 Author-email: jerry@skydio.com
 License: MIT
 Project-URL: Source, https://github.com/skydio/revup
 Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
@@ -28,30 +28,30 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
 
-  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/revup_light.svg"/>
+  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/revup_light.svg"/>
 
 </p>
 
 <p align="center">
 <a href="https://github.com/Skydio/revup"><img alt="Source Code" src="https://img.shields.io/badge/source-code-blue"/></a>
 <a href="https://github.com/Skydio/revup/issues"><img alt="Issues" src="https://img.shields.io/badge/issue-tracker-blue"/></a>
 <img alt="Python 3.8 | 3.9 | 3.10" src="https://img.shields.io/pypi/pyversions/revup"/>
 <a href="https://pypi.org/project/revup/"><img alt="PyPI" src="https://img.shields.io/pypi/v/revup"/></a>
 <a href="https://github.com/Skydio/revup/tree/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/pypi/l/revup"/></a>
 </p>
 
 Revup provides command-line tools that allow developers to iterate faster on parallel changes and reduce the overhead of creating and maintaining code reviews.
 
 <p align="center">
-<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif"/>
+<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_1.gif"/>
 </p>
 
 # Features
 
 - Revup creates multiple independent chains of branches for you in the background and without touching your working tree. It then creates and manages github pull requests for all those branches.
 - Pull requests target the actual base branch and can be merged manually or by continuous integration
 - Rebase detection saves time and continuous integration cost by not re-pushing if the patch hasn't changed
@@ -95,19 +95,20 @@
 Clone a sandbox repo by [forking](https://github.com/Skydio/revup/fork) revup, creating a [new](https://github.com/new) repo, or using some other repo you own.
 Creating test PRs can be spammy so don't do the tutorial on other people's repos.
 
 ```sh
 git clone https://github.com/<your-name>/revup.git && cd revup
 ```
 
-On first run, revup will prompt you to add github credentials
+On first run, you will need to configure github credentials. Create a personal access token [here](https://github.com/settings/tokens/new)
+and check the box for "full repo permissions". Revup needs this in order to create and modify pull requests. Then run
 ```sh
-revup upload
+revup config github_oauth
 ```
-Create a personal access token [here](https://github.com/settings/tokens/new) and check the box for "full repo permissions". Revup needs this in order to create and modify pull requests.
+and copy and paste the oauth into the prompt.
 
 ## Create independent pull requests
 
 Make your first two commits that will become two separate pull requests.
 Note the "Topic:" tag in the commit message - this is what causes revup to recognize and act on a commit.
 Each separately named topic will become a new pull request.
 
@@ -116,34 +117,34 @@
 git commit -m "My first revup foo" -m "Topic: foo"
 echo peh > bar; git add bar
 git commit -m "My first revup bar" -m "Topic: bar"
 
 revup upload
 ```
 
-![tutorial_1](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif)
+![tutorial_1](https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_1.gif)
 
 You've uploaded your first revup changes! Notice how in github, both branches target 'main'. This allows them to be merged independently.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/bar_github.png" width="50%">
+<img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/bar_github.png" width="50%">
 
 Under the hood, revup creates and pushes these branches for you, tracking and managing the dependencies as needed.
 
 ## Create relative pull requests
 
 Now we'll make a new review that's relative to "foo". The "Relative" tag will ensure the new review targets the correct branch.
 
 ```sh
 echo deh >> foo; git add foo
 git commit -m "My second revup foo" -m "Topic: foo2" -m "Relative: foo"
 
 revup upload
 ```
 
-![tutorial_2](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif)
+![tutorial_2](https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_2.gif)
 
 With this simple but powerful model, you can upload independent and dependent changes all at once.
 
 - Multiple commits can be in one topic, in which case they will all be in a single pull request.
 - Commits in the same topic do not need to be adjacent in history.
 - Topics relative to each other do not need to be adjacent in history, but the second topic must come after the first.
 
@@ -157,15 +158,15 @@
 revup amend HEAD~ --no-edit  # Specify a commit to amend
 # or
 revup amend bar --no-edit  # Specify a topic name to amend
 
 revup upload
 ```
 
-![tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_3.gif)
+![tutorial_3](https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_3.gif)
 
 `revup amend` makes it easy to modify commits in your history. You also have other options for modifying reviews:
 
 - Adding new commits with the same topic
 - Using `git rebase --interactive` along with `git commit --amend`
 
 ## Pulling in upstream changes
@@ -238,19 +239,19 @@
 revup upload --base-branch custom-branch-name
 ```
 
 ## Review graph and patchsets
 
 Revup will add 2 comments in every pull request to provide helpful features for users and reviewers. These are enabled by default and automatically updated as the pull request changes.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/review_graph.png" width="40%">
+<img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/review_graph.png" width="40%">
 
 The review graph provides links and titles to all local pull requests that have a relative relationship with the current pull request, including any that it depends on, or that depend on it. This allows you to quickly browse between pull requests in a chain.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png" width="80%">
+<img src="https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/patchsets.png" width="80%">
 
 The patchsets table provides a history of uploads for a given pull request as well as links and summaries of the diff between each upload. Notably, revup specially handles
 the case where you rebase then upload and will show you a diff with upstream files excluded.
 
 # Configuring revup
 
 Revup is highly configurable using a standard config file format. Every flag is also a config option, so users can get the exact behavior they need.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revup Version: 0.2.0 Summary: Revolutionary github
+Metadata-Version: 2.1 Name: revup Version: 0.2.1 Summary: Revolutionary github
 tools. Effortlessly create multiple branches and pull requests. Home-page:
 https://github.com/skydio/revup Author: Jerry Zhang Author-email:
 jerry@skydio.com License: MIT Project-URL: Source, https://github.com/skydio/
 revup Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
 Keywords: github python git workflow version-control python3 developer-tools
 code-review pull-requests developers developer-productivity stacked-diffs
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -41,45 +41,46 @@
 can also build from source to get the latest updates. ``` git clone https://
 github.com/Skydio/revup.git && cd revup make deps && make package && make
 install ``` # Tutorial This tutorial will guide you through using basic revup
 features. ## First time setup Clone a sandbox repo by [forking](https://
 github.com/Skydio/revup/fork) revup, creating a [new](https://github.com/new)
 repo, or using some other repo you own. Creating test PRs can be spammy so
 don't do the tutorial on other people's repos. ```sh git clone https://
-github.com//revup.git && cd revup ``` On first run, revup will prompt you to
-add github credentials ```sh revup upload ``` Create a personal access token
-[here](https://github.com/settings/tokens/new) and check the box for "full repo
-permissions". Revup needs this in order to create and modify pull requests. ##
-Create independent pull requests Make your first two commits that will become
-two separate pull requests. Note the "Topic:" tag in the commit message - this
-is what causes revup to recognize and act on a commit. Each separately named
-topic will become a new pull request. ```sh echo meh > foo; git add foo git
-commit -m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git
-commit -m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1]
-(https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
-tutorial_1.gif) You've uploaded your first revup changes! Notice how in github,
-both branches target 'main'. This allows them to be merged independently.
-[https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
-foo_github.png][https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
-images/bar_github.png] Under the hood, revup creates and pushes these branches
-for you, tracking and managing the dependencies as needed. ## Create relative
-pull requests Now we'll make a new review that's relative to "foo". The
-"Relative" tag will ensure the new review targets the correct branch. ```sh
-echo deh >> foo; git add foo git commit -m "My second revup foo" -m "Topic:
-foo2" -m "Relative: foo" revup upload ``` ![tutorial_2](https://
-raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif) With
+github.com//revup.git && cd revup ``` On first run, you will need to configure
+github credentials. Create a personal access token [here](https://github.com/
+settings/tokens/new) and check the box for "full repo permissions". Revup needs
+this in order to create and modify pull requests. Then run ```sh revup config
+github_oauth ``` and copy and paste the oauth into the prompt. ## Create
+independent pull requests Make your first two commits that will become two
+separate pull requests. Note the "Topic:" tag in the commit message - this is
+what causes revup to recognize and act on a commit. Each separately named topic
+will become a new pull request. ```sh echo meh > foo; git add foo git commit -
+m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git commit -
+m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1](https://
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_1.gif)
+You've uploaded your first revup changes! Notice how in github, both branches
+target 'main'. This allows them to be merged independently. [https://
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/foo_github.png]
+[https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/
+bar_github.png] Under the hood, revup creates and pushes these branches for
+you, tracking and managing the dependencies as needed. ## Create relative pull
+requests Now we'll make a new review that's relative to "foo". The "Relative"
+tag will ensure the new review targets the correct branch. ```sh echo deh >>
+foo; git add foo git commit -m "My second revup foo" -m "Topic: foo2" -
+m "Relative: foo" revup upload ``` ![tutorial_2](https://
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/tutorial_2.gif) With
 this simple but powerful model, you can upload independent and dependent
 changes all at once. - Multiple commits can be in one topic, in which case they
 will all be in a single pull request. - Commits in the same topic do not need
 to be adjacent in history. - Topics relative to each other do not need to be
 adjacent in history, but the second topic must come after the first. ## Modify
 pull requests Now let's update a pull request. ```sh echo heh >> bar; git add
 bar # Either revup amend HEAD~ --no-edit # Specify a commit to amend # or revup
 amend bar --no-edit # Specify a topic name to amend revup upload ``` !
-[tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
+[tutorial_3](https://raw.githubusercontent.com/skydio/revup/917438e/docs/
 images/tutorial_3.gif) `revup amend` makes it easy to modify commits in your
 history. You also have other options for modifying reviews: - Adding new
 commits with the same topic - Using `git rebase --interactive` along with `git
 commit --amend` ## Pulling in upstream changes Use `git pull --rebase` to pull
 in changes. Don't use `git merge` or `git pull` without rebase as this creates
 a merge commit. By default revup will not upload if you pull but haven't made
 changes to a commit. To override this and upload always, run `revup upload --
@@ -110,20 +111,20 @@
 latter case). ``` A fix for multiple branches Topic: fix Branches: main, rel1.1
 ``` You can specify base branch on the command line as well, although this is
 usually not necessary unless you're working on a branch that the autodetector
 doesn't know about (see Repo config below). ``` revup upload --base-branch
 custom-branch-name ``` ## Review graph and patchsets Revup will add 2 comments
 in every pull request to provide helpful features for users and reviewers.
 These are enabled by default and automatically updated as the pull request
-changes. [https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
+changes. [https://raw.githubusercontent.com/skydio/revup/917438e/docs/images/
 review_graph.png] The review graph provides links and titles to all local pull
 requests that have a relative relationship with the current pull request,
 including any that it depends on, or that depend on it. This allows you to
 quickly browse between pull requests in a chain. [https://
-raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png] The
+raw.githubusercontent.com/skydio/revup/917438e/docs/images/patchsets.png] The
 patchsets table provides a history of uploads for a given pull request as well
 as links and summaries of the diff between each upload. Notably, revup
 specially handles the case where you rebase then upload and will show you a
 diff with upstream files excluded. # Configuring revup Revup is highly
 configurable using a standard config file format. Every flag is also a config
 option, so users can get the exact behavior they need. Flags specified on the
 command line take precedence, followed by config in `~/.revupconfig`, followed
```

### Comparing `revup-0.2.0/revup.egg-info/SOURCES.txt` & `revup-0.2.1/revup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/setup.cfg` & `revup-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/setup.py` & `revup-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `revup-0.2.0/tests/test_tools.py` & `revup-0.2.1/tests/test_tools.py`

 * *Files identical despite different names*

