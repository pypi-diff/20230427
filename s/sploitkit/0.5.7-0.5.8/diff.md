# Comparing `tmp/sploitkit-0.5.7.tar.gz` & `tmp/sploitkit-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sploitkit-0.5.7.tar", last modified: Sun Nov 13 12:07:19 2022, max compression
+gzip compressed data, was "sploitkit-0.5.8.tar", last modified: Thu Apr 27 21:42:33 2023, max compression
```

## Comparing `sploitkit-0.5.7.tar` & `sploitkit-0.5.8.tar`

### file list

```diff
@@ -1,56 +1,123 @@
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)    35823 2021-04-23 12:54:37.000000 sploitkit-0.5.7/LICENSE
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     8702 2022-11-13 12:07:19.144654 sploitkit-0.5.7/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     7725 2022-02-08 10:47:55.000000 sploitkit-0.5.7/README.md
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1344 2022-11-13 12:07:19.148654 sploitkit-0.5.7/setup.cfg
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       64 2021-04-23 12:54:37.000000 sploitkit-0.5.7/setup.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        7 2022-11-13 11:53:51.000000 sploitkit-0.5.7/sploitkit/VERSION.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      347 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/__info__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1640 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2943 2021-09-11 17:42:18.000000 sploitkit-0.5.7/sploitkit/__main__.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit/base/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        0 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/__init__.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit/base/commands/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        0 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/commands/__init__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     8544 2021-06-03 18:18:16.000000 sploitkit-0.5.7/sploitkit/base/commands/general.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     3302 2021-09-12 08:00:35.000000 sploitkit-0.5.7/sploitkit/base/commands/module.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     4664 2022-03-01 14:19:49.000000 sploitkit-0.5.7/sploitkit/base/commands/project.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     2339 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/commands/recording.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1189 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/commands/root.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1397 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/commands/session.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     7359 2022-03-25 23:10:31.000000 sploitkit-0.5.7/sploitkit/base/commands/utils.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit/base/models/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        0 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/models/__init__.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      823 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/models/notes.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1374 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/models/organization.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)      921 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/models/systems.py
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1065 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/base/models/users.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit/core/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)       56 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1248 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/application.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)    12332 2021-09-12 08:00:44.000000 sploitkit-0.5.7/sploitkit/core/command.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit/core/components/
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      263 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/__init__.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4213 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/completer.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)    21118 2022-11-06 18:00:26.000000 sploitkit-0.5.7/sploitkit/core/components/config.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      689 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/defaults.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4987 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/files.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     4492 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/jobs.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)      551 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/layout.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3553 2021-06-03 10:49:34.000000 sploitkit-0.5.7/sploitkit/core/components/logger.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1055 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/recorder.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     2482 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/sessions.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     5388 2021-04-23 12:54:37.000000 sploitkit-0.5.7/sploitkit/core/components/store.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     1689 2021-06-01 22:08:38.000000 sploitkit-0.5.7/sploitkit/core/components/validator.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)    24786 2022-03-25 23:09:55.000000 sploitkit-0.5.7/sploitkit/core/console.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)    32317 2022-03-25 23:04:57.000000 sploitkit-0.5.7/sploitkit/core/entity.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     3267 2021-06-01 15:19:27.000000 sploitkit-0.5.7/sploitkit/core/model.py
--rwxrwxr-x   0 morfal    (1000) morfal    (1000)     7287 2021-09-11 19:38:52.000000 sploitkit-0.5.7/sploitkit/core/module.py
-drwxrwxr-x   0 morfal    (1000) morfal    (1000)        0 2022-11-13 12:07:19.144654 sploitkit-0.5.7/sploitkit.egg-info/
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     8702 2022-11-13 12:07:18.000000 sploitkit-0.5.7/sploitkit.egg-info/PKG-INFO
--rw-rw-r--   0 morfal    (1000) morfal    (1000)     1420 2022-11-13 12:07:19.000000 sploitkit-0.5.7/sploitkit.egg-info/SOURCES.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)        1 2022-11-13 12:07:18.000000 sploitkit-0.5.7/sploitkit.egg-info/dependency_links.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       54 2022-11-13 12:07:18.000000 sploitkit-0.5.7/sploitkit.egg-info/entry_points.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       59 2022-11-13 12:07:18.000000 sploitkit-0.5.7/sploitkit.egg-info/requires.txt
--rw-rw-r--   0 morfal    (1000) morfal    (1000)       10 2022-11-13 12:07:18.000000 sploitkit-0.5.7/sploitkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.849548 sploitkit-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-27 21:42:21.000000 sploitkit-0.5.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.825546 sploitkit-0.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.829546 sploitkit-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-27 21:42:21.000000 sploitkit-0.5.8/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-27 21:42:21.000000 sploitkit-0.5.8/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-27 21:42:21.000000 sploitkit-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 21:42:21.000000 sploitkit-0.5.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 21:42:21.000000 sploitkit-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48518 2023-04-27 21:42:33.845548 sploitkit-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-27 21:42:22.000000 sploitkit-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.829546 sploitkit-0.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/coverage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.829546 sploitkit-0.5.8/docs/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.829546 sploitkit-0.5.8/docs/pages/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/base/commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/base/consoles.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/base/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/base.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.833547 sploitkit-0.5.8/docs/pages/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/classes/command.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/classes/console.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/classes/datastore.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/classes/entity.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/classes/module.md
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/classes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/design.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.833547 sploitkit-0.5.8/docs/pages/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/examples/dronesploit.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.837547 sploitkit-0.5.8/docs/pages/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   159466 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/class-hierarchy.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1418966 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/classes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/command-key-completion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/command-validation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/command-value-completion.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/console-prompt.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50410 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/dronesploit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31324 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/my-sploit-start.png
+-rw-r--r--   0 runner    (1001) docker     (123)   235170 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/packages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    96565 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/img/under-construction.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.837547 sploitkit-0.5.8/docs/pages/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/js/collapsible-navbar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/pages/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-27 21:42:21.000000 sploitkit-0.5.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-27 21:42:21.000000 sploitkit-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 21:42:21.000000 sploitkit-0.5.8/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 21:42:21.000000 sploitkit-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:42:33.849548 sploitkit-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.825546 sploitkit-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.837547 sploitkit-0.5.8/src/sploitkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2943 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.837547 sploitkit-0.5.8/src/sploitkit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.841547 sploitkit-0.5.8/src/sploitkit/base/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/config.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.841547 sploitkit-0.5.8/src/sploitkit/base/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/models/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/models/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/base/models/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.841547 sploitkit-0.5.8/src/sploitkit/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      866 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/application.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12289 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.845548 sploitkit-0.5.8/src/sploitkit/core/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4199 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/completer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21118 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4987 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4492 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/layout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3542 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/recorder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5388 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/store.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1600 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/components/validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24851 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32317 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3267 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-27 21:42:21.000000 sploitkit-0.5.8/src/sploitkit/core/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.837547 sploitkit-0.5.8/src/sploitkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48518 2023-04-27 21:42:33.000000 sploitkit-0.5.8/src/sploitkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-27 21:42:33.000000 sploitkit-0.5.8/src/sploitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:42:33.000000 sploitkit-0.5.8/src/sploitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 21:42:33.000000 sploitkit-0.5.8/src/sploitkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 21:42:33.000000 sploitkit-0.5.8/src/sploitkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:42:33.000000 sploitkit-0.5.8/src/sploitkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.845548 sploitkit-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-27 21:42:21.000000 sploitkit-0.5.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.845548 sploitkit-0.5.8/testsploit/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 21:42:21.000000 sploitkit-0.5.8/testsploit/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.845548 sploitkit-0.5.8/testsploit/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-27 21:42:21.000000 sploitkit-0.5.8/testsploit/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 21:42:21.000000 sploitkit-0.5.8/testsploit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.845548 sploitkit-0.5.8/testsploit/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-27 21:42:21.000000 sploitkit-0.5.8/testsploit/modules/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 21:42:21.000000 sploitkit-0.5.8/testsploit/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:42:33.845548 sploitkit-0.5.8/testsploit/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)   262144 2023-04-27 21:42:21.000000 sploitkit-0.5.8/testsploit/workspace/store.db
```

### Comparing `sploitkit-0.5.7/LICENSE` & `sploitkit-0.5.8/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `sploitkit-0.5.7/README.md` & `sploitkit-0.5.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-<p align="center"><img src="https://github.com/dhondta/python-sploitkit/raw/master/docs/logo.png"></p>
+<p align="center"><img src="https://github.com/dhondta/python-sploitkit/raw/main/docs/pages/img/logo.png"></p>
 <h1 align="center">SploitKit <a href="https://twitter.com/intent/tweet?text=SploitKit%20-%20Devkit%20for%20building%20Metasploit-like%20consoles.%0D%0APython%20library%20for%20easilly%20building%20framework%20consoles%20in%20a%20Metasploit-like%20style%20with%20a%20comprehensive%20API.%0D%0Ahttps%3a%2f%2fgithub%2ecom%2fdhondta%2fpython-sploitkit%0D%0A&hashtags=python,programming,devkit,framework,console,ctftools"><img src="https://img.shields.io/badge/Tweet--lightgrey?logo=twitter&style=social" alt="Tweet" height="20"/></a></h1>
 <h3 align="center">Make a Metasploit-like console.</h3>
 
 [![PyPi](https://img.shields.io/pypi/v/sploitkit.svg)](https://pypi.python.org/pypi/sploitkit/)
 [![Read The Docs](https://readthedocs.org/projects/python-sploitkit/badge/?version=latest)](https://python-sploitkit.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.com/dhondta/python-sploitkit.svg?branch=master)](https://travis-ci.com/dhondta/python-sploitkit)
-[![Coverage Status](https://coveralls.io/repos/github/dhondta/python-sploitkit/badge.svg?branch=master)](https://coveralls.io/github/dhondta/python-sploitkit?branch=master)
+[![Build Status](https://github.com/dhondta/python-sploitkit/actions/workflows/python-package.yml/badge.svg)](https://github.com/dhondta/python-sploitkit/actions/workflows/python-package.yml)
+[![Coverage Status](https://raw.githubusercontent.com/dhondta/python-sploitkit/main/docs/coverage.svg)](#)
 [![Python Versions](https://img.shields.io/pypi/pyversions/sploitkit.svg)](https://pypi.python.org/pypi/sploitkit/)
-[![Requirements Status](https://requires.io/github/dhondta/python-sploitkit/requirements.svg?branch=master)](https://requires.io/github/dhondta/python-sploitkit/requirements/?branch=master)
 [![Known Vulnerabilities](https://snyk.io/test/github/dhondta/python-sploitkit/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/dhondta/python-sploitkit?targetFile=requirements.txt)
 [![License](https://img.shields.io/pypi/l/sploitkit.svg)](https://pypi.python.org/pypi/sploitkit/)
-[![Donate](https://img.shields.io/badge/donate-paypal-orange.svg)](https://www.paypal.me/dhondta)
 
 
 This toolkit is aimed to easilly build framework consoles in a Metasploit-like style. It provides a comprehensive interface to define CLI commands, modules and models for its storage database.
 
 ```
 pip install sploitkit
 ```
 
-## :sunglasses: Usage
+## Usage
 
 From this point, `main.py` has the following code:
 
 ```python
 #!/usr/bin/python3
 from sploitkit import FrameworkConsole
 
@@ -38,54 +36,47 @@
         "MySploit",
         #TODO: configure your console settings
     ).start()
 ```
 
 And you can run it from the terminal:
 
-![](https://github.com/dhondta/python-sploitkit/tree/master/docs/img/my-sploit-start.png)
+![](https://github.com/dhondta/python-sploitkit/tree/main/docs/pages/img/my-sploit-start.png)
 
-## :ballot_box_with_check: Features
+## Features
 
 Sploitkit provides a base set of entities (consoles, commands, modules, models).
 
 Multiple base console levels already exist (for detailed descriptions, see [the console section](../console/index.html)):
 
-- [`FrameworkConsole`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/console.py): the root console, started through `main.py`
-- [`ProjectConsole`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/project.py): the project console, for limiting the workspace to a single project, invoked through the `select [project]` command
-- [`ModuleConsole`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/module.py): the module console, started when a module is invoked through the `use [module]` command
+- [`FrameworkConsole`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/console.py): the root console, started through `main.py`
+- [`ProjectConsole`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/project.py): the project console, for limiting the workspace to a single project, invoked through the `select [project]` command
+- [`ModuleConsole`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/module.py): the module console, started when a module is invoked through the `use [module]` command
 
 This framework provides more than 20 base commands, distributed in sets of functionalities (for detailed descriptions, see [the command section](../command/index.html)):
 
-- [*general*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/general.py): commands for every level (e.g. `help`, `show`, `set`)
-- [*module*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/module.py): base module-level commands (e.g. `use`, `run`, `show`)
-- [*project*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/project.py): base project-level commands (e.g. `select`, `load`, `archive`)
-- [*recording*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/recording.py): recording commands, for managing `.rc` files (`record`, `replay`)
-- [*root*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/root.py): base root-level commands (`help`)
-- [*utils*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/utils.py): utility commands (`shell`, `pydbg`, `memory`)
+- [*general*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/general.py): commands for every level (e.g. `help`, `show`, `set`)
+- [*module*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/module.py): base module-level commands (e.g. `use`, `run`, `show`)
+- [*project*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/project.py): base project-level commands (e.g. `select`, `load`, `archive`)
+- [*recording*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/recording.py): recording commands, for managing `.rc` files (`record`, `replay`)
+- [*root*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/root.py): base root-level commands (`help`)
+- [*utils*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/utils.py): utility commands (`shell`, `pydbg`, `memory`)
 
 It also holds some base models for its storage:
 
-- [*users*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/models/notes.py): for user-related data (`User`, `Email`, `Password`)
-- [*systems*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/models/systems.py): for system-related data (`Host`, `Port`, `Service`)
-- [*organization*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/models/organization.py): for organization-related data (`Organization`, `Unit`, `Employee`)
-- [*notes*](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/models/notes.py): for linking notes to users, hosts or organizations
+- [*users*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/models/notes.py): for user-related data (`User`, `Email`, `Password`)
+- [*systems*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/models/systems.py): for system-related data (`Host`, `Port`, `Service`)
+- [*organization*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/models/organization.py): for organization-related data (`Organization`, `Unit`, `Employee`)
+- [*notes*](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/models/notes.py): for linking notes to users, hosts or organizations
 
 No module is provided with the framework as it is case-specific.
 
-## :pencil2: Customization
+## Customization
 
 Sploitkit defines multiple types of entities for various purposes. The following entities can be subclassed:
 
-- [`Console`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/console.py): a new console for a new level of interaction (e.g. [`ProjectConsole`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/project.py)) ; the "`root`" level is owned by the [`FrameworkConsole`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/console.py), [`Console`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/console.py) shall be used to create new subconsoles, to be called by commands from the root console (see an example [here](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/module.py) for the module-level commands with [`ModuleConsole(Console)` and `Use(Command)`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/commands/module.py))
-- [`Command`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/command.py): a new command associated with any or defined consoles using the `level` attribute
-- [`Module`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/module.py): a new module associated to a console
-- [`Model`, `BaseModel`, `StoreExtension`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/core/model.py): respectively for new models, their association tables and store additional methods (e.g. [`User(Model)`, `Email(Model)`, `UserEmail(BaseModel)`, `UsersStorage(StoreExtension)`](https://github.com/dhondta/python-sploitkit/blob/master/sploitkit/base/models/users.py))
+- [`Console`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/console.py): a new console for a new level of interaction (e.g. [`ProjectConsole`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/project.py)) ; the "`root`" level is owned by the [`FrameworkConsole`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/console.py), [`Console`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/console.py) shall be used to create new subconsoles, to be called by commands from the root console (see an example [here](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/module.py) for the module-level commands with [`ModuleConsole(Console)` and `Use(Command)`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/commands/module.py))
+- [`Command`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/command.py): a new command associated with any or defined consoles using the `level` attribute
+- [`Module`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/module.py): a new module associated to a console
+- [`Model`, `BaseModel`, `StoreExtension`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/core/model.py): respectively for new models, their association tables and store additional methods (e.g. [`User(Model)`, `Email(Model)`, `UserEmail(BaseModel)`, `UsersStorage(StoreExtension)`](https://github.com/dhondta/python-sploitkit/blob/main/sploitkit/base/models/users.py))
 
 
-## :clap:  Supporters
-
-[![Stargazers repo roster for @dhondta/python-sploitkit](https://reporoster.com/stars/dark/dhondta/python-sploitkit)](https://github.com/dhondta/python-sploitkit/stargazers)
-
-[![Forkers repo roster for @dhondta/python-sploitkit](https://reporoster.com/forks/dark/dhondta/python-sploitkit)](https://github.com/dhondta/python-sploitkit/network/members)
-
-<p align="center"><a href="#"><img src="https://img.shields.io/badge/Back%20to%20top--lightgrey?style=social" alt="Back to top" height="20"/></a></p>
```

### Comparing `sploitkit-0.5.7/sploitkit/__init__.py` & `sploitkit-0.5.8/src/sploitkit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import os
 import re
 from ipaddress import ip_address
 from peewee import *
 from peewee import __all__ as _peewee
-from shutil import which
-from subprocess import call
-from tempfile import TemporaryFile
 from tinyscript.helpers.path import Path
 
 from .core import *
 from .core import __all__ as _core
 from .core.console import print_formatted_text
```

### Comparing `sploitkit-0.5.7/sploitkit/__main__.py` & `sploitkit-0.5.8/src/sploitkit/__main__.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/general.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/general.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/module.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/module.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/project.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/project.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/recording.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/recording.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/root.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/root.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/session.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/session.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/commands/utils.py` & `sploitkit-0.5.8/src/sploitkit/base/commands/utils.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/models/notes.py` & `sploitkit-0.5.8/src/sploitkit/base/models/notes.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/models/organization.py` & `sploitkit-0.5.8/src/sploitkit/base/models/organization.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/models/systems.py` & `sploitkit-0.5.8/src/sploitkit/base/models/systems.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/base/models/users.py` & `sploitkit-0.5.8/src/sploitkit/base/models/users.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/command.py` & `sploitkit-0.5.8/src/sploitkit/core/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: UTF-8 -*-
-import gc
 import re
 from inspect import getfullargspec
-from tinyscript import logging
 from tinyscript.helpers import failsafe, BorderlessTable, Path, PythonPath
 
 from .components.config import Config
 from .components.logger import get_logger
 from .entity import Entity, MetaEntity
```

### Comparing `sploitkit-0.5.7/sploitkit/core/components/completer.py` & `sploitkit-0.5.8/src/sploitkit/core/components/completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: UTF-8 -*-
-import shlex
 from prompt_toolkit.completion import Completer, Completion
 
 
 __all__ = ["CommandCompleter"]
 
 
 def _filter_sort(lst, prefix=None, sort=False):
```

### Comparing `sploitkit-0.5.7/sploitkit/core/components/config.py` & `sploitkit-0.5.8/src/sploitkit/core/components/config.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/defaults.py` & `sploitkit-0.5.8/src/sploitkit/core/components/defaults.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/files.py` & `sploitkit-0.5.8/src/sploitkit/core/components/files.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/jobs.py` & `sploitkit-0.5.8/src/sploitkit/core/components/jobs.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/layout.py` & `sploitkit-0.5.8/src/sploitkit/core/components/layout.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/logger.py` & `sploitkit-0.5.8/src/sploitkit/core/components/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf8 -*-
-import re
 from logging.handlers import RotatingFileHandler
 from termcolor import colored
 from tinyscript import logging
 
 
 __all__ = ["get_logger", "null_logger", "set_logging_level"]
```

### Comparing `sploitkit-0.5.7/sploitkit/core/components/recorder.py` & `sploitkit-0.5.8/src/sploitkit/core/components/recorder.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/sessions.py` & `sploitkit-0.5.8/src/sploitkit/core/components/sessions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 import os
 import shlex
 import shutil
-from subprocess import Popen, PIPE
+from subprocess import Popen
 from tinyscript.helpers import Path
 
 __all__ = ["SessionsManager"]
 
 
 class Session(object):
     """ Class representing a session object based on a shell command """
```

### Comparing `sploitkit-0.5.7/sploitkit/core/components/store.py` & `sploitkit-0.5.8/src/sploitkit/core/components/store.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/components/validator.py` & `sploitkit-0.5.8/src/sploitkit/core/components/validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-# -*- coding: UTF-8 -*-
-import shlex
-from inspect import getargspec
-from prompt_toolkit.validation import Validator, ValidationError
-
-
-__all__ = ["CommandValidator"]
-
-
-class CommandValidator(Validator):
-    """ Completer for console's commands and arguments. """
-    def __init__(self, fail=True):
-        self._fail = fail
-        super(CommandValidator, self).__init__()
-    
-    def validate(self, document):
-        # first, tokenize document.text
-        tokens = self.console._get_tokens(document.text.strip())
-        l = len(tokens)
-        # then handle tokens
-        commands = self.console.commands
-        # when no token provided, do nothing
-        if l == 0:
-            return
-        # when a command is being typed, mention if it is existing
-        cmd = tokens[0]
-        if l == 1 and cmd not in commands.keys() and self._fail:
-            raise ValidationError(message="Unknown command")
-        # when a valid first token is provided, handle command's validation, if any available
-        elif l >= 1 and cmd in commands.keys():
-            c = commands[cmd]._instance
-            try:
-                c._validate(*tokens[1:])
-            except Exception as e:
-                m = "Command syntax: %s{}" % c.signature.format(cmd)
-                e = str(e)
-                if not e.startswith("validate() "):
-                    m = m.format([" (" + e + ")", ""][len(e) == 0])
-                else:
-                    m = m.format("")
-                raise ValidationError(message=m)
-        # otherwise, the command is considered bad
-        elif self._fail:
-            raise ValidationError(message="Bad command")
-
+# -*- coding: UTF-8 -*-
+from prompt_toolkit.validation import Validator, ValidationError
+
+
+__all__ = ["CommandValidator"]
+
+
+class CommandValidator(Validator):
+    """ Completer for console's commands and arguments. """
+    def __init__(self, fail=True):
+        self._fail = fail
+        super(CommandValidator, self).__init__()
+    
+    def validate(self, document):
+        # first, tokenize document.text
+        tokens = self.console._get_tokens(document.text.strip())
+        l = len(tokens)
+        # then handle tokens
+        commands = self.console.commands
+        # when no token provided, do nothing
+        if l == 0:
+            return
+        # when a command is being typed, mention if it is existing
+        cmd = tokens[0]
+        if l == 1 and cmd not in commands.keys() and self._fail:
+            raise ValidationError(message="Unknown command")
+        # when a valid first token is provided, handle command's validation, if any available
+        elif l >= 1 and cmd in commands.keys():
+            c = commands[cmd]._instance
+            try:
+                c._validate(*tokens[1:])
+            except Exception as e:
+                m = "Command syntax: %s{}" % c.signature.format(cmd)
+                e = str(e)
+                if not e.startswith("validate() "):
+                    m = m.format([" (" + e + ")", ""][len(e) == 0])
+                else:
+                    m = m.format("")
+                raise ValidationError(message=m)
+        # otherwise, the command is considered bad
+        elif self._fail:
+            raise ValidationError(message="Bad command")
+
```

### Comparing `sploitkit-0.5.7/sploitkit/core/console.py` & `sploitkit-0.5.8/src/sploitkit/core/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,18 @@
     
     def play(self, *commands, capture=False):
         """ Execute a list of commands. """
         global _output
         if capture:
             r = []
         error = False
-        w, _ = get_terminal_size()
+        try:
+            w, _ = get_terminal_size()
+        except TypeError:
+            w = 80
         for c in commands:
             if capture:
                 if error:
                     r.append((c, None, None))
                     continue
                 __tmp = _output
                 _output = _CaptureOutput()
```

### Comparing `sploitkit-0.5.7/sploitkit/core/entity.py` & `sploitkit-0.5.8/src/sploitkit/core/entity.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/model.py` & `sploitkit-0.5.8/src/sploitkit/core/model.py`

 * *Files identical despite different names*

### Comparing `sploitkit-0.5.7/sploitkit/core/module.py` & `sploitkit-0.5.8/src/sploitkit/core/module.py`

 * *Files identical despite different names*

