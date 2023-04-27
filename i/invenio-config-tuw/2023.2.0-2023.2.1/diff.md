# Comparing `tmp/invenio-config-tuw-2023.2.0.tar.gz` & `tmp/invenio-config-tuw-2023.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.2.0.tar", last modified: Mon Apr 24 16:22:47 2023, max compression
+gzip compressed data, was "invenio-config-tuw-2023.2.1.tar", last modified: Thu Apr 27 16:00:07 2023, max compression
```

## Comparing `invenio-config-tuw-2023.2.0.tar` & `invenio-config-tuw-2023.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.893079 invenio-config-tuw-2023.2.0/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2221 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5158 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.901080 invenio-config-tuw-2023.2.0/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.901080 invenio-config-tuw-2023.2.0/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.905080 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8631 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6700 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1104 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.905080 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5158 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.115030 invenio-config-tuw-2023.2.1/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.1/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2301 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.1/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5238 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio-config-tuw-2023.2.1/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.119030 invenio-config-tuw-2023.2.1/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6700 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1104 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-11 13:14:29.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:03:59.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5238 2023-04-27 16:00:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-04-27 16:00:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-27 16:00:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-04-27 16:00:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-27 16:00:06.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-04-27 16:00:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-04-27 16:00:07.000000 invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.1/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-27 16:00:07.123030 invenio-config-tuw-2023.2.1/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.1/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.1/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.0/.editorconfig` & `invenio-config-tuw-2023.2.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/.tx/config` & `invenio-config-tuw-2023.2.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/CHANGES.rst` & `invenio-config-tuw-2023.2.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ..
-    Copyright (C) 2020-2022 TU Wien.
+    Copyright (C) 2020-2023 TU Wien.
 
-    Invenio-Config-TUW is free software; you can redistribute it and/or
+    Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24)
+Version 2023.2 (released 2023-04-24, updated 2023-04-27)
 
 - v11 compat: Update permission policies and disable archive download
+- Set affiliation (hard-coded) to TU Wien in `user.profile`
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.0/CONTRIBUTING.rst` & `invenio-config-tuw-2023.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/LICENSE` & `invenio-config-tuw-2023.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/MANIFEST.in` & `invenio-config-tuw-2023.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/PKG-INFO` & `invenio-config-tuw-2023.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.0
+Version: 2023.2.1
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -85,26 +85,27 @@
 --------------------
 
 Last but not least, we also set some default configuration values for deployments
 of InvenioRDM at TU Wien.
 The relevant files here are ``config.py`` and ``ext.py``.
 
 ..
-    Copyright (C) 2020-2022 TU Wien.
+    Copyright (C) 2020-2023 TU Wien.
 
-    Invenio-Config-TUW is free software; you can redistribute it and/or
+    Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24)
+Version 2023.2 (released 2023-04-24, updated 2023-04-27)
 
 - v11 compat: Update permission policies and disable archive download
+- Set affiliation (hard-coded) to TU Wien in `user.profile`
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.0/README.rst` & `invenio-config-tuw-2023.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/babel.ini` & `invenio-config-tuw-2023.2.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/docs/Makefile` & `invenio-config-tuw-2023.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/docs/conf.py` & `invenio-config-tuw-2023.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/docs/index.rst` & `invenio-config-tuw-2023.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/docs/make.bat` & `invenio-config-tuw-2023.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/__init__.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/config.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/handlers.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2022 TU Wien.
+# Copyright (C) 2020-2023 TU Wien.
 #
-# Invenio-Config-TUW is free software; you can redistribute it and/or modify
+# Invenio Config TUW is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Custom handlers for the Keycloak integration."""
 
 
 from flask import current_app, redirect, render_template, request, session, url_for
 from flask_login import current_user
@@ -210,14 +210,18 @@
                 user.username = create_username_from_info(user_info)
 
             # update the full name if it has changed
             old_profile = user.user_profile or {}
             if new_full_name and new_full_name != user.user_profile["full_name"]:
                 user.user_profile = {"full_name": new_full_name, **old_profile}
 
+        # Hard code the affiliation to TU Wien, since we are currently not accepting any externals.
+        # It is set on every login.
+        user.user_profile = {**user.user_profile, "affiliations": "TU Wien"}
+
         # Link account
         # ------------
         # Need to store token in database instead of only the session when
         # called first time.
         token = response_token_setter(remote, resp)
 
     # Setup account
```

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/utils.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/config.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/ext.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/formatters.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/formatters.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/forms.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/__init__.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/generators.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/policies.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/permissions/policies.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/startup.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/startup.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw/utils.py` & `invenio-config-tuw-2023.2.1/invenio_config_tuw/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/PKG-INFO` & `invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.0
+Version: 2023.2.1
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -85,26 +85,27 @@
 --------------------
 
 Last but not least, we also set some default configuration values for deployments
 of InvenioRDM at TU Wien.
 The relevant files here are ``config.py`` and ``ext.py``.
 
 ..
-    Copyright (C) 2020-2022 TU Wien.
+    Copyright (C) 2020-2023 TU Wien.
 
-    Invenio-Config-TUW is free software; you can redistribute it and/or
+    Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24)
+Version 2023.2 (released 2023-04-24, updated 2023-04-27)
 
 - v11 compat: Update permission policies and disable archive download
+- Set affiliation (hard-coded) to TU Wien in `user.profile`
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio-config-tuw-2023.2.1/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/setup.cfg` & `invenio-config-tuw-2023.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/tests/conftest.py` & `invenio-config-tuw-2023.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.0/tests/test_invenio_config_tuw.py` & `invenio-config-tuw-2023.2.1/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*

