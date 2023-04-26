# Comparing `tmp/autocalver-2022.8.11.62018.tar.gz` & `tmp/autocalver-2023.4.26.74472rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocalver-2022.8.11.62018.tar", last modified: Thu Aug 11 17:18:02 2022, max compression
+gzip compressed data, was "autocalver-2023.4.26.74472rc1.tar", last modified: Wed Apr 26 20:42:16 2023, max compression
```

## Comparing `autocalver-2022.8.11.62018.tar` & `autocalver-2023.4.26.74472rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 developer  (1000) root         (0)        0 2022-08-11 17:18:02.945351 autocalver-2022.8.11.62018/
--rw-r--r--   0 developer  (1000) root         (0)     1051 2022-07-10 17:46:58.000000 autocalver-2022.8.11.62018/LICENSE
--rw-r--r--   0 developer  (1000) root         (0)       21 2022-08-11 15:56:18.000000 autocalver-2022.8.11.62018/MANIFEST.in
--rw-r--r--   0 developer  (1000) root         (0)      128 2022-08-11 17:18:02.945351 autocalver-2022.8.11.62018/PKG-INFO
--rw-r--r--   0 developer  (1000) root         (0)     3125 2022-08-11 16:04:19.000000 autocalver-2022.8.11.62018/README.md
--rw-r--r--   0 developer  (1000) root         (0)      241 2022-08-11 17:17:46.000000 autocalver-2022.8.11.62018/git-log-head
--rw-r--r--   0 developer  (1000) root         (0)      173 2022-07-10 17:46:58.000000 autocalver-2022.8.11.62018/pyproject.toml
--rw-r--r--   0 developer  (1000) root         (0)      511 2022-08-11 17:18:02.949351 autocalver-2022.8.11.62018/setup.cfg
--rw-r--r--   0 developer  (1000) root         (0)       37 2022-07-10 17:46:58.000000 autocalver-2022.8.11.62018/setup.py
-drwxr-xr-x   0 developer  (1000) root         (0)        0 2022-08-11 17:18:02.925352 autocalver-2022.8.11.62018/src/
-drwxr-xr-x   0 developer  (1000) root         (0)        0 2022-08-11 17:18:02.937352 autocalver-2022.8.11.62018/src/autocalver/
--rw-r--r--   0 developer  (1000) root         (0)        0 2022-07-10 17:46:58.000000 autocalver-2022.8.11.62018/src/autocalver/__init__.py
--rw-r--r--   0 developer  (1000) root         (0)     3089 2022-08-11 17:15:43.000000 autocalver-2022.8.11.62018/src/autocalver/integration.py
-drwxr-xr-x   0 developer  (1000) root         (0)        0 2022-08-11 17:18:02.945351 autocalver-2022.8.11.62018/src/autocalver.egg-info/
--rw-r--r--   0 developer  (1000) root         (0)      128 2022-08-11 17:18:02.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1000) root         (0)      396 2022-08-11 17:18:02.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1000) root         (0)        1 2022-08-11 17:18:02.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1000) root         (0)      167 2022-08-11 17:18:02.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1000) root         (0)       86 2022-08-11 17:18:02.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/requires.txt
--rw-r--r--   0 developer  (1000) root         (0)       11 2022-08-11 17:18:02.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/top_level.txt
--rw-r--r--   0 developer  (1000) root         (0)        1 2022-07-10 17:50:39.000000 autocalver-2022.8.11.62018/src/autocalver.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:42:16.791323 autocalver-2023.4.26.74472rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-26 20:42:16.791323 autocalver-2023.4.26.74472rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-26 20:42:15.000000 autocalver-2023.4.26.74472rc1/git-log-head
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:42:16.791323 autocalver-2023.4.26.74472rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:42:16.787323 autocalver-2023.4.26.74472rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:42:16.787323 autocalver-2023.4.26.74472rc1/src/autocalver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/src/autocalver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/src/autocalver/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:42:16.791323 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-26 20:42:16.000000 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 20:42:16.000000 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:42:16.000000 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 20:42:16.000000 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 20:42:16.000000 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:42:16.000000 autocalver-2023.4.26.74472rc1/src/autocalver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:42:16.791323 autocalver-2023.4.26.74472rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-04-26 20:41:56.000000 autocalver-2023.4.26.74472rc1/tests/test_integration.py
```

### Comparing `autocalver-2022.8.11.62018/LICENSE` & `autocalver-2023.4.26.74472rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `autocalver-2022.8.11.62018/README.md` & `autocalver-2023.4.26.74472rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ## Configuration
 
 The right way to make sure
 `autocalver`
 is installed is to require it in
 `pyproject.toml`:
 
-```
+```toml
 [build-system]
 requires = ["setuptools>=45", "wheel", "autocalver"]
 ```
 
 Note that
 `autocalver`
 will
@@ -45,16 +45,16 @@
 run a command to pull a prefix of the commit log,
 and save it to a file.
 For example,
 with
 `git`,
 you can use
 
-```
-$ git log -n 1 --date=iso > git-log-head
+```shell
+git log -n 1 --date=iso > git-log-head
 ```
 
 One advantage of separating the stages like that is that it is possible
 to have the package builder itself running in an environent that does not
 have access to the version control metadata,
 only the source files and the prefix of the commit log.
 Failing to produce the log will cause the package build to fail.
@@ -63,15 +63,15 @@
 `setup.cfg`.
 Configuration is done via
 `pyproject.toml`.
 For example,
 a configuration appropriate to
 pipeline CI might be:
 
-```
+```toml
 [tool.autocalver]
 use = true
 log = "git-log-head"
 is_main_var = "BUILD_BRANCH_REF"
 is_main_match = ".*/main$"
 ```
 
@@ -101,27 +101,27 @@
 With this configuration,
 the following versions will be produced
 (asssuming the time of the latest commit is
 October 10, 2021, 8:39:44 in Pacific time).
 
 Local build:
 
-```
+```console
 $ python -m build -n --wheel 2>& 1| tail -1
 Successfully built fake_package-2021.10.10.56384.dev1-py3-none-any.whl
 ```
 
 Note that the version has a
 `dev1`
 in its name.
 
 
 Simulate tagged build:
 
-```
+```console
 $ GITHUB_REF=refs/tags/test-fix-PROJ-121 python -m build -n --wheel 2>& 1| tail -1
 Successfully built fake_package-2021.10.10.56384rc1-py3-none-any.whl
 ```
 
 This version has an
 `rc1`
 in the name,
@@ -130,24 +130,24 @@
 and test fixes.
 However,
 since tag pushes are not reviewed,
 these do not produce releases.
 
 Simulate merge to main:
 
-```
+```console
 $ GITHUB_REF=refs/heads/main python -m build -n --wheel 2>& 1| tail -1
 Successfully built fake_package-2021.10.10.56384-py3-none-any.whl
 ```
 
 Note that without
-:code:`use = true`,
+`use = true`,
 the tool will not replace the version.
 If
-:code:`use = true`
+`use = true`
 is there,
 missing any of the other variables
 will cause an
 *error*
 during the build,
 as a non-existing build
 is better than a broken when.
```

### Comparing `autocalver-2022.8.11.62018/src/autocalver/integration.py` & `autocalver-2023.4.26.74472rc1/src/autocalver/integration.py`

 * *Files identical despite different names*

