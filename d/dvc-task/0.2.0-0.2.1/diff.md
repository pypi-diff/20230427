# Comparing `tmp/dvc-task-0.2.0.tar.gz` & `tmp/dvc-task-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-task-0.2.0.tar", last modified: Tue Feb 28 08:49:19 2023, max compression
+gzip compressed data, was "dvc-task-0.2.1.tar", last modified: Thu Apr 27 09:22:22 2023, max compression
```

## Comparing `dvc-task-0.2.0.tar` & `dvc-task-0.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.324511 dvc-task-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-02-28 08:48:55.000000 dvc-task-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-28 08:48:55.000000 dvc-task-0.2.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-02-28 08:48:55.000000 dvc-task-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-02-28 08:48:55.000000 dvc-task-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-02-28 08:49:19.324511 dvc-task-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-02-28 08:48:55.000000 dvc-task-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-02-28 08:48:55.000000 dvc-task-0.2.0/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-28 08:48:55.000000 dvc-task-0.2.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-28 08:48:55.000000 dvc-task-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-28 08:48:55.000000 dvc-task-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-28 08:48:55.000000 dvc-task-0.2.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-28 08:48:55.000000 dvc-task-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-28 08:49:19.324511 dvc-task-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.316511 dvc-task-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/src/dvc_task/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/src/dvc_task/app/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/app/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/src/dvc_task/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/contrib/kombu_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/src/dvc_task/proc/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/proc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/proc/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/proc/process.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/proc/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.324511 dvc-task-0.2.0/src/dvc_task/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-02-28 08:48:55.000000 dvc-task-0.2.0/src/dvc_task/worker/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.320511 dvc-task-0.2.0/src/dvc_task.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-02-28 08:49:19.000000 dvc-task-0.2.0/src/dvc_task.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-28 08:49:19.000000 dvc-task-0.2.0/src/dvc_task.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 08:49:19.000000 dvc-task-0.2.0/src/dvc_task.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 08:49:19.000000 dvc-task-0.2.0/src/dvc_task.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-28 08:49:19.000000 dvc-task-0.2.0/src/dvc_task.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-28 08:49:19.000000 dvc-task-0.2.0/src/dvc_task.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.324511 dvc-task-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.324511 dvc-task-0.2.0/tests/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/app/test_filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.324511 dvc-task-0.2.0/tests/proc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/proc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/proc/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/proc/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/proc/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/test_dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 08:49:19.324511 dvc-task-0.2.0/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-02-28 08:48:55.000000 dvc-task-0.2.0/tests/worker/test_temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.130275 dvc-task-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-27 09:21:37.000000 dvc-task-0.2.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-27 09:21:37.000000 dvc-task-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-27 09:21:37.000000 dvc-task-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-27 09:22:22.138275 dvc-task-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-27 09:21:37.000000 dvc-task-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-27 09:21:37.000000 dvc-task-0.2.1/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-27 09:21:37.000000 dvc-task-0.2.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 09:21:37.000000 dvc-task-0.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 09:21:37.000000 dvc-task-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-27 09:21:37.000000 dvc-task-0.2.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-27 09:21:37.000000 dvc-task-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 09:22:22.138275 dvc-task-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.130275 dvc-task-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/app/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/contrib/kombu_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/worker/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:22:21.000000 dvc-task-0.2.1/src/dvc_task.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/app/test_filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/test_dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/worker/test_temporary.py
```

### Comparing `dvc-task-0.2.0/.cruft.json` & `dvc-task-0.2.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/.github/dependabot.yml` & `dvc-task-0.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/.github/workflows/docs.yml` & `dvc-task-0.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/.github/workflows/release.yml` & `dvc-task-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/.github/workflows/tests.yml` & `dvc-task-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/.gitignore` & `dvc-task-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/.pre-commit-config.yaml` & `dvc-task-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/CODE_OF_CONDUCT.rst` & `dvc-task-0.2.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/CONTRIBUTING.rst` & `dvc-task-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/LICENSE` & `dvc-task-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/PKG-INFO` & `dvc-task-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-task
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extensible task queue used in DVC.
 Home-page: https://github.com/iterative/dvc-task
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-task-0.2.0/README.rst` & `dvc-task-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/docs/assets/logo.svg` & `dvc-task-0.2.1/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/docs/gen_ref_pages.py` & `dvc-task-0.2.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/mkdocs.yml` & `dvc-task-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/noxfile.py` & `dvc-task-0.2.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/pyproject.toml` & `dvc-task-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/setup.cfg` & `dvc-task-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task/app/filesystem.py` & `dvc-task-0.2.1/src/dvc_task/app/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,33 +240,54 @@
         def _delete_expired(
             msg: Message,
             queues: Set[str],
             now: float,
             cache: Dict[str, str],
             include_tickets: bool = False,
         ):
+            assert isinstance(msg.properties, dict)
+            properties = cast(Dict[str, Any], msg.properties)
+            delivery_info: Dict[str, str] = properties.get("delivery_info", {})
             if queues:
-                assert isinstance(msg.properties, dict)
-                properties = cast(Dict[str, Any], msg.properties)
-                delivery_info: Dict[str, str] = properties.get("delivery_info", {})
                 routing_key = delivery_info.get("routing_key")
                 if routing_key and routing_key in queues:
                     return
             headers = cast(Dict[str, Any], msg.headers)
             expires: Optional[float] = headers.get("expires")
             ticket = msg.headers.get("ticket")
             if include_tickets and ticket or (expires is not None and expires <= now):
                 assert msg.delivery_tag
-                self._delete_msg(msg.delivery_tag, [], cache)
+                try:
+                    self._delete_msg(msg.delivery_tag, [], cache)
+                except ValueError:
+                    pass
 
         queues = set(exclude) if exclude else set()
         now = datetime.now().timestamp()
         for msg in self._iter_data_folder():
             _delete_expired(msg, queues, now, self._queued_msg_path_cache)
         for msg in self._iter_processed_folder():
             _delete_expired(
                 msg, queues, now, self._processed_msg_path_cache, include_tickets=True
             )
 
     def clean(self):
         """Clean extraneous celery messages from this FSApp."""
         self._gc(exclude=[self.conf.task_default_queue])
+        self._clean_pidbox(f"reply.{self.conf.task_default_queue}.pidbox")
+
+    def _clean_pidbox(self, exchange: str):
+        """Clean pidbox replies for the specified exchange."""
+
+        def _delete_replies(msg: Message, exchange: str, cache: Dict[str, str]):
+            assert isinstance(msg.properties, dict)
+            properties = cast(Dict[str, Any], msg.properties)
+            delivery_info: Dict[str, str] = properties.get("delivery_info", {})
+            if delivery_info.get("exchange", "") == exchange:
+                assert msg.delivery_tag
+                try:
+                    self._delete_msg(msg.delivery_tag, [], cache)
+                except ValueError:
+                    pass
+
+        for msg in self._iter_data_folder():
+            _delete_replies(msg, exchange, self._queued_msg_path_cache)
```

### Comparing `dvc-task-0.2.0/src/dvc_task/contrib/kombu_filesystem.py` & `dvc-task-0.2.1/src/dvc_task/contrib/kombu_filesystem.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task/proc/exceptions.py` & `dvc-task-0.2.1/src/dvc_task/proc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task/proc/manager.py` & `dvc-task-0.2.1/src/dvc_task/proc/manager.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task/proc/process.py` & `dvc-task-0.2.1/src/dvc_task/proc/process.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task/utils.py` & `dvc-task-0.2.1/src/dvc_task/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task/worker/temporary.py` & `dvc-task-0.2.1/src/dvc_task/worker/temporary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Temporary worker module."""
 import logging
 import os
 import threading
 import time
-from typing import Any, List, Mapping
+from typing import Any, Dict, List, Mapping, Optional
 
 from celery import Celery
 from celery.utils.nodenames import default_nodename
 
 from dvc_task.app.filesystem import FSApp
 
 logger = logging.getLogger(__name__)
@@ -32,41 +32,53 @@
         Additional keyword arguments will be passed as celery worker
         configuration.
         """
         self.app = app
         self.timeout = timeout
         self.config = kwargs
 
+    def ping(self, name: str, timeout: float = 1.0) -> Optional[List[Dict[str, Any]]]:
+        """Ping the specified worker."""
+        return self._ping(destination=[default_nodename(name)], timeout=timeout)
+
+    def _ping(
+        self, *, destination: Optional[List[str]] = None, timeout: float = 1.0
+    ) -> Optional[List[Dict[str, Any]]]:
+        return self.app.control.ping(destination=destination, timeout=timeout)
+
     def start(self, name: str, fsapp_clean: bool = False) -> None:
         """Start the worker if it does not already exist.
 
         Runs the Celery worker main thread in the current process.
 
         Arguments:
             name: Celery worker name.
             fsapp_clean: Automatically cleanup FSApp broker on shutdown. Has no
                 effect unless app is an FSApp instance.
         """
         if os.name == "nt":
             # see https://github.com/celery/billiard/issues/247
             os.environ["FORKED_BY_MULTIPROCESSING"] = "1"
 
-        if not self.app.control.ping(destination=[name]):
+        if not self.ping(name):
             monitor = threading.Thread(
                 target=self.monitor,
                 daemon=True,
                 args=(name,),
-                kwargs={"fsapp_clean": fsapp_clean},
             )
             monitor.start()
             config = dict(self.config)
             config["hostname"] = name
             argv = ["worker"]
             argv.extend(self._parse_config(config))
             self.app.worker_main(argv=argv)
+            if fsapp_clean and isinstance(self.app, FSApp):  # type: ignore[unreachable]
+                logger.info("cleaning up FSApp broker.")
+                self.app.clean()
+            logger.info("done")
 
     @staticmethod
     def _parse_config(config: Mapping[str, Any]) -> List[str]:
         loglevel = config.get("loglevel", "info")
         argv = [f"--loglevel={loglevel}"]
         for key in ("hostname", "pool", "concurrency", "prefetch_multiplier"):
             value = config.get(key)
@@ -81,41 +93,36 @@
             if config.get(key):
                 argv_key = key.replace("_", "-")
                 argv.append(f"--{argv_key}")
         if config.get("task_events"):
             argv.append("-E")
         return argv
 
-    def monitor(self, name: str, fsapp_clean: bool = False) -> None:
+    def monitor(self, name: str) -> None:
         """Monitor the worker and stop it when the queue is empty."""
-        logger.debug("monitor: waiting for worker to start")
         nodename = default_nodename(name)
-        while not self.app.control.ping(destination=[nodename]):
-            # wait for worker to start
-            time.sleep(1)
 
         def _tasksets(nodes):
             for taskset in (
                 nodes.active(),
                 nodes.scheduled(),
                 nodes.reserved(),
             ):
                 if taskset is not None:
                     yield from taskset.values()
 
             if isinstance(self.app, FSApp):
                 yield from self.app.iter_queued()
 
-        logger.info("monitor: watching celery worker '%s'", nodename)
-        while self.app.control.ping(destination=[nodename]):
+        logger.debug("monitor: watching celery worker '%s'", nodename)
+        while True:
             time.sleep(self.timeout)
             nodes = self.app.control.inspect(  # type: ignore[call-arg]
-                destination=[nodename]
+                destination=[nodename],
+                limit=1,
             )
             if nodes is None or not any(tasks for tasks in _tasksets(nodes)):
                 logger.info("monitor: shutting down due to empty queue.")
-                self.app.control.shutdown(destination=[nodename])
                 break
-        if fsapp_clean and isinstance(self.app, FSApp):
-            logger.info("monitor: cleanup FSApp broker.")
-            self.app.clean()
-        logger.info("monitor: done")
+        logger.debug("monitor: sending shutdown to '%s'.", nodename)
+        self.app.control.shutdown()
+        logger.debug("monitor: done")
```

### Comparing `dvc-task-0.2.0/src/dvc_task.egg-info/PKG-INFO` & `dvc-task-0.2.1/src/dvc_task.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-task
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extensible task queue used in DVC.
 Home-page: https://github.com/iterative/dvc-task
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-task-0.2.0/src/dvc_task.egg-info/SOURCES.txt` & `dvc-task-0.2.1/src/dvc_task.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/src/dvc_task.egg-info/requires.txt` & `dvc-task-0.2.1/src/dvc_task.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/tests/app/test_filesystem.py` & `dvc-task-0.2.1/tests/app/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/tests/proc/conftest.py` & `dvc-task-0.2.1/tests/proc/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/tests/proc/test_manager.py` & `dvc-task-0.2.1/tests/proc/test_manager.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/tests/proc/test_process.py` & `dvc-task-0.2.1/tests/proc/test_process.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/tests/proc/test_tasks.py` & `dvc-task-0.2.1/tests/proc/test_tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.0/tests/worker/test_temporary.py` & `dvc-task-0.2.1/tests/worker/test_temporary.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     name = "worker1@localhost"
     worker.start(name)
     _args, kwargs = worker_cls.call_args
     assert kwargs["hostname"] == name
     assert kwargs["pool"] == TaskPool
     assert kwargs["concurrency"] == 1
     assert kwargs["prefetch_multiplier"] == 1
-    thread.assert_called_once_with(
-        target=worker.monitor, daemon=True, args=(name,), kwargs={"fsapp_clean": False}
-    )
+    thread.assert_called_once_with(target=worker.monitor, daemon=True, args=(name,))
 
 
 @pytest.mark.flaky(
     max_runs=3,
     rerun_filter=lambda *args: sys.platform == "darwin",
 )
 def test_start_already_exists(
```

