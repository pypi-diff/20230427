# Comparing `tmp/invenio-rdm-migrator-1.0.0a5.tar.gz` & `tmp/invenio-rdm-migrator-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a5.tar", last modified: Mon Apr 24 20:54:20 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a6.tar", last modified: Thu Apr 27 15:51:32 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a5.tar` & `invenio-rdm-migrator-1.0.0a6.tar`

### file list

```diff
@@ -1,102 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/extract/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 15:51:31.000000 invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:51:32.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-27 15:51:23.000000 invenio-rdm-migrator-1.0.0a6/tests/streams/test_cache.py
```

### Comparing `invenio-rdm-migrator-1.0.0a5/.editorconfig` & `invenio-rdm-migrator-1.0.0a6/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-1.0.0a6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/.github/workflows/tests.yml` & `invenio-rdm-migrator-1.0.0a6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/CONTRIBUTING.rst` & `invenio-rdm-migrator-1.0.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/LICENSE` & `invenio-rdm-migrator-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/MANIFEST.in` & `invenio-rdm-migrator-1.0.0a6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/PKG-INFO` & `invenio-rdm-migrator-1.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a5/README.rst` & `invenio-rdm-migrator-1.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/docs/Makefile` & `invenio-rdm-migrator-1.0.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/docs/conf.py` & `invenio-rdm-migrator-1.0.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/docs/index.rst` & `invenio-rdm-migrator-1.0.0a6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/docs/make.bat` & `invenio-rdm-migrator-1.0.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/models.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/postgresql.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/load/postgresql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 CERN.
+# Copyright (C) 2022-2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """PostgreSQL load module."""
 
 
 import contextlib
 import csv
 import json
 from abc import ABC, abstractmethod
 from dataclasses import fields
 from datetime import datetime
 from pathlib import Path
-from uuid import UUID, uuid4
+from uuid import UUID
 
 import psycopg
 from invenio_records.dictutils import dict_set  # TODO: can we do without?
 
 from .base import Load
 
 
@@ -41,44 +41,53 @@
                 val = val.isoformat()
             elif issubclass(f.type, (UUID,)):
                 val = str(val)
         row.append(val)
     return row
 
 
-def generate_uuid(data):
-    """Generate a UUID."""
-    return str(uuid4())
-
-
-class PostgreSQLCopyLoad(Load):  # TODO: abstract SQL from PostgreSQL?
+class PostgreSQLCopyLoad(Load):
     """PostgreSQL COPY load."""
 
-    def __init__(self, db_uri, table_loads, tmp_dir):
+    def __init__(self, db_uri, table_generators, tmp_dir):
         """Constructor."""
         self.db_uri = db_uri
         self.tmp_dir = Path(tmp_dir) / f"tables{_ts(iso=False)}"
-        self.table_loads = table_loads
+        self.table_generators = table_generators
 
     def _cleanup(self, db=False):
         """Cleanup csv files and DB after load."""
-        for table in self.table_loads:
+        for table in self.table_generators:
             table.cleanup(db=db)
 
     def _prepare(self, entries):
         """Dump entries in csv files for COPY command."""
         self.tmp_dir.mkdir(parents=True, exist_ok=True)
 
-        _prepared_tables = []
-        for table in self.table_loads:
-            # otherwise the generator is exhausted by the first table
-            # TODO: nested generators, how expensive is this copy op?
-            _prepared_tables.extend(table.prepare(self.tmp_dir, entries=entries))
+        # use this context manager to close all opened files at once
+        with contextlib.ExitStack() as stack:
+            output_files = {}
+            for entry in entries:
+                for tg in self.table_generators:
+                    tg.prepare(self.tmp_dir, entry, stack, output_files)
+
+            for tg in self.table_generators:
+                tg.post_prepare(self.tmp_dir, stack, output_files)
 
-        return iter(_prepared_tables)  # yield at the end vs yield per table
+        prepared_tables = []
+        # FIXME: needs to preserve order
+        # the logic is very inefficient, maybe and ordered-set
+        # or change the data structure of tables to keep order information
+        # and hten process it
+        for tg in self.table_generators:
+            for table in tg.tables:
+                if table not in prepared_tables:
+                    prepared_tables.append(table)
+
+        return iter(prepared_tables)  # yield at the end vs yield per table
 
     def _load(self, table_entries):
         """Bulk load CSV table files.
 
         Loads the tables in the order given by the generator.
         """
         with psycopg.connect(self.db_uri) as conn:
@@ -130,48 +139,53 @@
 
 
 class TableGenerator(ABC):
     """Create CSV files with table create and inserts."""
 
     def __init__(self, tables, pks=None):
         """Constructor."""
-        self._tables = tables
+        self.tables = tables
         self.pks = pks or []
 
     @abstractmethod
     def _generate_rows(self, **kwargs):
         """Yield generated rows."""
         pass
 
     @abstractmethod
     def cleanup(self, **kwargs):
         """Cleanup."""
         pass
 
-    def _generate_pks(self, data):
+    def _generate_pks(self, data, create=False):
+        keys = data.keys()
         for path, pk_func in self.pks:
-            dict_set(data, path, pk_func(data))
+            try:
+                root = path.split(".")[0]
+                # avoids creating e.g. "record" in a draft and generating a recid + uuid
+                if create or root in keys:
+                    dict_set(data, path, pk_func(data))
+            except KeyError:
+                print(f"Path {path} not found on record")
 
     def _resolve_references(self, data, **kwargs):
         """Resolve references e.g communities slug names."""
         pass
 
-    def prepare(self, tmp_dir, entries, **kwargs):
+    def prepare(self, tmp_dir, entry, stack, output_files, **kwargs):
         """Compute rows."""
-        # use this context manager to close all opened files at once
-        with contextlib.ExitStack() as stack:
-            out_files = {}
-            for entry in entries:
-                # is_db_empty would come in play and make _generate_pks optional
-                self._generate_pks(entry)
-                # resolve entry references
-                self._resolve_references(entry)
-                for entry in self._generate_rows(entry):
-                    if entry._table_name not in out_files:
-                        fpath = tmp_dir / f"{entry._table_name}.csv"
-                        out_files[entry._table_name] = csv.writer(
-                            stack.enter_context(open(fpath, "w+"))
-                        )
-                    writer = out_files[entry._table_name]
-                    writer.writerow(as_csv_row(entry))
+        # is_db_empty would come in play and make _generate_pks optional
+        self._generate_pks(entry, kwargs.get("create", False))
+        # resolve entry references
+        self._resolve_references(entry)
+        for entry in self._generate_rows(entry):
+            if entry._table_name not in output_files:
+                fpath = tmp_dir / f"{entry._table_name}.csv"
+                output_files[entry._table_name] = csv.writer(
+                    stack.enter_context(open(fpath, "w+"))
+                )
+            writer = output_files[entry._table_name]
+            writer.writerow(as_csv_row(entry))
 
-        return self._tables
+    def post_prepare(self, tmp_dir, stack, output_files, **kwargs):
+        """Create rows after iterating over the entries."""
+        pass
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/load.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration users load module."""
 
 from ...load import PostgreSQLCopyLoad
-from .table_generator import CommunityTableGenerator
+from .table_generator import UserTableGenerator
 
 
-class CommunityCopyLoad(PostgreSQLCopyLoad):
-    """PostgreSQL communities COPY load."""
+class UserCopyLoad(PostgreSQLCopyLoad):
+    """PostgreSQL users COPY load."""
 
-    def __init__(self, cache, db_uri=None, tmp_dir=None):
+    def __init__(self, db_uri=None, tmp_dir=None, cache=None):
         """Constructor."""
-        self.communities_cache = cache.get("communities", {})
         super().__init__(
             db_uri=db_uri,
-            table_loads=[
-                CommunityTableGenerator(communities_cache=self.communities_cache),
+            table_generators=[
+                UserTableGenerator(),
             ],
             tmp_dir=tmp_dir,
         )
 
     def _validate(self):
         """Validate data before loading."""
         return True
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/models.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class FilesCopyLoad(PostgreSQLCopyLoad):
     """PostgreSQL files COPY load."""
 
     def __init__(self, db_uri=None, tmp_dir=None, cache=None):
         """Constructor."""
         super().__init__(
             db_uri=db_uri,
-            table_loads=[
+            table_generators=[
                 FilesTableGenerator(),
             ],
             tmp_dir=tmp_dir,
         )
 
     def _validate(self):
         """Validate data before loading."""
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/models.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/models.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/table_generator.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/table_generators/records.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,70 +3,31 @@
 # Copyright (C) 2022 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration record table load module."""
 
-
-import random
 from datetime import datetime
+from uuid import UUID
 
-from ...load.models import PersistentIdentifier
-from ...load.postgresql import TableGenerator, generate_uuid
-from ..communities.models import RDMParentCommunityMetadata
-from .models import RDMParentMetadata, RDMRecordFile, RDMRecordMetadata, RDMVersionState
-
-
-class RDMVersionStateTableGenerator(TableGenerator):
-    """RDM version state computed table."""
-
-    def __init__(self, parent_cache):
-        """Constructor."""
-        super().__init__(tables=[RDMVersionState])
-        self.parent_cache = parent_cache
-
-    def _generate_rows(self, parent_entry, **kwargs):
-        # Version state to be populated in the end from the final state
-        yield RDMVersionState(
-            latest_index=parent_entry["version"]["latest_index"],
-            parent_id=parent_entry["id"],
-            latest_id=parent_entry["version"]["latest_id"],
-            next_draft_id=None,
-        )
-
-    def prepare(self, tmp_dir, entries, **kwargs):
-        """Overwrite entries with parent cache entries."""
-        return super().prepare(tmp_dir, self.parent_cache.values(), **kwargs)
-
-    def cleanup(self, **kwargs):
-        """Cleanup."""
-        pass
-
-
-# keep track of generated PKs, since there's a chance they collide
-GENERATED_PID_PKS = set()
-
-
-def _pid_pk():
-    while True:
-        # we start at 1M to avoid collisions with existing low-numbered PKs
-        val = random.randint(1_000_000, 2_147_483_647 - 1)
-        if val not in GENERATED_PID_PKS:
-            GENERATED_PID_PKS.add(val)
-            return val
-
-
-def _generate_recid(data):
-    return {
-        "pk": _pid_pk(),
-        "obj_type": "rec",
-        "pid_type": "recid",
-        "status": "R",
-    }
+from ....load.ids import generate_recid, generate_uuid, pid_pk
+from ....load.models import PersistentIdentifier
+from ....load.postgresql import TableGenerator, _ts
+from ...communities.models import RDMParentCommunityMetadata
+from ..models import RDMParentMetadata, RDMRecordFile, RDMRecordMetadata
+from .parents import generate_parent_rows
+
+
+def _is_valid_uuid(value):
+    try:
+        UUID(value)
+        return True
+    except:
+        return False
 
 
 def generate_files_uuids(data):
     """Generate uuid for every file in the list.
 
     Return the transformed list with the generated ids.
     """
@@ -81,142 +42,155 @@
     _id = data.get("id")
     return _id if _id else generate_uuid(None)
 
 
 class RDMRecordTableGenerator(TableGenerator):
     """RDM Record and related tables load."""
 
-    def __init__(self, parent_cache, communities_cache):
+    def __init__(self, parents_cache, records_cache, communities_cache):
         """Constructor."""
         super().__init__(
             tables=[
                 PersistentIdentifier,
                 RDMParentMetadata,
                 RDMRecordMetadata,
                 RDMParentCommunityMetadata,
                 RDMRecordFile,
             ],
             pks=[
                 ("record.id", generate_record_uuid),
                 ("parent.id", generate_uuid),
-                ("record.json.pid", _generate_recid),
-                ("parent.json.pid", _generate_recid),
+                ("record.json.pid", generate_recid),
+                ("parent.json.pid", generate_recid),
                 ("record.parent_id", lambda d: d["parent"]["id"]),
                 ("record_files", generate_files_uuids),
             ],
         )
-        self.parent_cache = parent_cache
+        self.parents_cache = parents_cache
+        self.records_cache = records_cache
         self.communities_cache = communities_cache
 
     def _generate_rows(self, data, **kwargs):
+        """Generates rows for a record."""
         now = datetime.utcnow().isoformat()
+        parent = data["parent"]
+        record = data.get("record")
 
+        if not record:
+            return
+
+        record_pid = record["json"]["pid"]
+
+        # parent
+        cached_parent = self.parents_cache.get(parent["json"]["id"])
+        if not cached_parent:
+            self.parents_cache.add(
+                parent["json"]["id"],  # recid
+                {
+                    "id": parent["id"],
+                    "latest_index": record["index"],
+                    "latest_id": record["id"],
+                },
+            )
+            yield from generate_parent_rows(parent)
+            # parent community
+            if "default" in parent["json"]["communities"]:
+                parent_def_id = parent["json"]["communities"]["default"]
+                parent_comm_id = parent["id"]
+                # TODO temporary fix for deleted communities. When a community is deleted, its id is the slug and fails on DB (foreign key expects uuid and not string)
+                # check uuid
+                if _is_valid_uuid(parent_def_id) and _is_valid_uuid(parent_comm_id):
+                    yield RDMParentCommunityMetadata(
+                        community_id=parent_def_id,
+                        record_id=parent_comm_id,
+                        request_id=None,
+                    )
+                else:
+                    record_id = record["json"]["id"]
+                    print(
+                        f"[{_ts()}] Record parent community not migrated. Record id[{record_id}]. parent community [{parent_comm_id}] parent default community [{parent_def_id}]"
+                    )
+        else:
+            self.parents_cache.update(
+                parent["json"]["id"],
+                {
+                    "latest_index": record["index"],
+                    "latest_id": record["id"],
+                },
+            )
+
+        parent_id = cached_parent["id"] if cached_parent else record["parent_id"]
         # record
-        rec = data["record"]
-        record_pid = rec["json"]["pid"]
-        parent = data["parent"]
-        rec_parent_id = self.parent_cache.get(parent["json"]["id"], {}).get("id")
+        self.records_cache.add(
+            record["json"]["id"],  # recid
+            {
+                "index": record["index"],
+                "id": record["id"],  # uuid
+                "parent_id": parent_id,  # parent uuid
+                "fork_version_id": record["version_id"],
+            },
+        )
+
         yield RDMRecordMetadata(
-            id=rec["id"],
-            json=rec["json"],
-            created=rec["created"],
-            updated=rec["updated"],
-            version_id=rec["version_id"],
-            index=rec["index"],
-            bucket_id=rec.get("bucket_id"),
-            parent_id=rec_parent_id or rec["parent_id"],
+            id=record["id"],
+            json=record["json"],
+            created=record["created"],
+            updated=record["updated"],
+            version_id=record["version_id"],
+            index=record["index"],
+            bucket_id=record.get("bucket_id"),
+            parent_id=parent_id,
         )
         # recid
         yield PersistentIdentifier(
             id=record_pid["pk"],
             pid_type=record_pid["pid_type"],
-            pid_value=rec["json"]["id"],
+            pid_value=record["json"]["id"],
             status=record_pid["status"],
             object_type=record_pid["obj_type"],
-            object_uuid=rec["id"],
+            object_uuid=record["id"],
             created=now,
             updated=now,
         )
         # DOI
-        if "doi" in rec["json"]["pids"]:
+        if "doi" in record["json"]["pids"]:
             yield PersistentIdentifier(
-                id=_pid_pk(),
+                id=pid_pk(),
                 pid_type="doi",
-                pid_value=rec["json"]["pids"]["doi"]["identifier"],
+                pid_value=record["json"]["pids"]["doi"]["identifier"],
                 status="R",
                 object_type="rec",
-                object_uuid=rec["id"],
+                object_uuid=record["id"],
                 created=now,
                 updated=now,
             )
         # OAI
-        if "oai" in rec["json"]["pids"]:
+        if "oai" in record["json"]["pids"]:
             yield PersistentIdentifier(
-                id=_pid_pk(),
+                id=pid_pk(),
                 pid_type="oai",
-                pid_value=rec["json"]["pids"]["oai"]["identifier"],
+                pid_value=record["json"]["pids"]["oai"]["identifier"],
                 status="R",
                 object_type="rec",
-                object_uuid=rec["id"],
+                object_uuid=record["id"],
                 created=now,
                 updated=now,
             )
 
-        # parent
-        if parent["json"]["id"] not in self.parent_cache:
-            self.parent_cache[parent["json"]["id"]] = dict(
-                id=parent["id"],
-                version=dict(latest_index=rec["index"], latest_id=rec["id"]),
-            )
-            parent_pid = parent["json"]["pid"]
-            # record
-            yield RDMParentMetadata(
-                id=parent["id"],
-                json=parent["json"],
-                created=parent["created"],
-                updated=parent["updated"],
-                version_id=parent["version_id"],
-            )
-            # recid
-            yield PersistentIdentifier(
-                id=parent_pid["pk"],
-                pid_type=parent_pid["pid_type"],
-                pid_value=parent["json"]["id"],
-                status=parent_pid["status"],
-                object_type=parent_pid["obj_type"],
-                object_uuid=parent["id"],
-                created=now,
-                updated=now,
-            )
-            # parent community
-            if "default" in parent["json"]["communities"]:
-                yield RDMParentCommunityMetadata(
-                    community_id=parent["json"]["communities"]["default"],
-                    record_id=parent["id"],
-                    request_id=None,
-                )
-        else:
-            # parent in cache - update version
-            cached_parent = self.parent_cache[parent["json"]["id"]]
-            # check if current record is a new version of the cached one
-            if cached_parent["version"]["latest_index"] < rec["index"]:
-                cached_parent["version"] = dict(
-                    latest_index=rec["index"], latest_id=rec["id"]
-                )
         # record files
         record_files = data["record_files"]
         for _file in record_files:
             yield RDMRecordFile(
                 id=_file["id"],
                 json=_file["json"],
                 created=_file["created"],
                 updated=_file["updated"],
                 version_id=_file["version_id"],
                 key=_file["key"],
-                record_id=rec["id"],
+                record_id=record["id"],
                 object_version_id=_file["object_version_id"],
             )
 
     def _resolve_references(self, data, **kwargs):
         """Resolve references e.g communities slug names."""
 
         def _resolve_communities(communities):
@@ -263,15 +237,15 @@
         # RDMDraftMetadata.query.delete()
         # db.session.commit()
         pass
 
     def _cleanup_files(self):
         """Cleanup files after load."""
         # FIXME: tables does not return the name correct
-        # delegate to table_loads?
+        # delegate to table_generators?
         # for table in self.tables:
         #     fpath = self.tmp_dir / f"{table._table_name}.csv"
         #     print(f"Checking {fpath}")
         #     if fpath.exists():
         #         print(f"Deleting {fpath}")
         #         fpath.unlink(missing_ok=True)
         pass
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/records/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def __init__(self, cache, db_uri, tmp_dir):
         """Constructor."""
         self.communities_cache = cache.get("communities", {})
         super().__init__(
             db_uri=db_uri,
             tmp_dir=tmp_dir,
-            table_loads=[
+            table_generators=[
                 RequestTableGenerator(self.communities_cache),
             ],
         )
 
     def _validate(self):
         """Validate data before loading."""
         pass
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/models.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # Copyright (C) 2023 CERN.
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio RDM migration requests table load module."""
 
-from ...load.postgresql import TableGenerator, generate_uuid
+from ...load.ids import generate_uuid
+from ...load.postgresql import TableGenerator
 from .models import RequestMetadata
 
 
 class RequestTableGenerator(TableGenerator):
     """Requests and related tables load."""
 
     def __init__(self, communities_cache):
@@ -45,11 +46,15 @@
         """
         # it assumes the data is transformed by an InclusionRequestEntry
         request_slug = data["json"]["receiver"]["community"]
         community_id = self.communities_cache[request_slug]
 
         data["json"]["receiver"]["community"] = community_id
 
+    def prepare(self, tmp_dir, entry, stack, output_files, **kwargs):
+        """Compute rows."""
+        super().prepare(tmp_dir, entry, stack, output_files, create=True, **kwargs)
+
     def cleanup(self, **kwargs):
         """Cleanup."""
         # TODO
         pass
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """InvenioRDM migration streams runner."""
 
 import yaml
 
+from .cache import ParentsCache, RecordsCache
 from .streams import Stream
 
 
 class Runner:
     """ETL streams runner."""
 
     def _read_config(self, filepath):
@@ -29,15 +30,16 @@
             #     '<parent_pid>': {
             #         'id': <generated_parent_uuid>,
             #         'version': {
             #             'latest_index': 'record_index',
             #             'latest_id': 'record id',
             #         }
             # }
-            "parent": {},
+            "parents": ParentsCache(),
+            "records": RecordsCache(),
             "communities": {},
         }
         config = self._read_config(config_filepath)
 
         for definition in stream_definitions:
             stream_config = config.get(definition.name)
             if stream_config is not None:
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/streams.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/streams.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/models.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator/transform/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,7 +27,18 @@
 class Entry(ABC):
     """Base entry class."""
 
     @abstractmethod
     def transform(self, entry):
         """Transform entry."""
         pass
+
+
+def drop_nones(data):
+    """Recursively drop Nones in dict d and return a new dictionary."""
+    dd = {}
+    for k, v in data.items():
+        if isinstance(v, dict) and v:  # second clause removes empty dicts
+            dd[k] = drop_nones(v)
+        elif v is not None:
+            dd[k] = v
+    return dd
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-1.0.0a6/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 invenio_rdm_migrator.egg-info/not-zip-safe
 invenio_rdm_migrator.egg-info/requires.txt
 invenio_rdm_migrator.egg-info/top_level.txt
 invenio_rdm_migrator/extract/__init__.py
 invenio_rdm_migrator/extract/base.py
 invenio_rdm_migrator/load/__init__.py
 invenio_rdm_migrator/load/base.py
+invenio_rdm_migrator/load/ids.py
 invenio_rdm_migrator/load/models.py
 invenio_rdm_migrator/load/postgresql.py
 invenio_rdm_migrator/streams/__init__.py
+invenio_rdm_migrator/streams/cache.py
 invenio_rdm_migrator/streams/runner.py
 invenio_rdm_migrator/streams/streams.py
 invenio_rdm_migrator/streams/communities/__init__.py
 invenio_rdm_migrator/streams/communities/load.py
 invenio_rdm_migrator/streams/communities/models.py
 invenio_rdm_migrator/streams/communities/table_generator.py
 invenio_rdm_migrator/streams/communities/transform.py
@@ -48,29 +50,34 @@
 invenio_rdm_migrator/streams/files/load.py
 invenio_rdm_migrator/streams/files/models.py
 invenio_rdm_migrator/streams/files/table_generator.py
 invenio_rdm_migrator/streams/files/transform.py
 invenio_rdm_migrator/streams/records/__init__.py
 invenio_rdm_migrator/streams/records/load.py
 invenio_rdm_migrator/streams/records/models.py
-invenio_rdm_migrator/streams/records/table_generator.py
 invenio_rdm_migrator/streams/records/transform.py
+invenio_rdm_migrator/streams/records/table_generators/__init__.py
+invenio_rdm_migrator/streams/records/table_generators/drafts.py
+invenio_rdm_migrator/streams/records/table_generators/parents.py
+invenio_rdm_migrator/streams/records/table_generators/records.py
+invenio_rdm_migrator/streams/records/table_generators/versions.py
 invenio_rdm_migrator/streams/requests/__init__.py
 invenio_rdm_migrator/streams/requests/load.py
 invenio_rdm_migrator/streams/requests/models.py
 invenio_rdm_migrator/streams/requests/table_generator.py
 invenio_rdm_migrator/streams/requests/transform.py
 invenio_rdm_migrator/streams/users/__init__.py
 invenio_rdm_migrator/streams/users/load.py
 invenio_rdm_migrator/streams/users/models.py
 invenio_rdm_migrator/streams/users/table_generator.py
 invenio_rdm_migrator/streams/users/transform.py
 invenio_rdm_migrator/transform/__init__.py
 invenio_rdm_migrator/transform/base.py
 tests/conftest.py
+tests/streams/test_cache.py
 tests/streams/communities/conftest.py
 tests/streams/communities/test_communities_load.py
 tests/streams/communities/test_communities_table_generator.py
 tests/streams/communities/test_communities_transform.py
 tests/streams/files/conftest.py
 tests/streams/files/test_files_load.py
 tests/streams/files/test_files_table_generator.py
```

### Comparing `invenio-rdm-migrator-1.0.0a5/run-tests.sh` & `invenio-rdm-migrator-1.0.0a6/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/setup.cfg` & `invenio-rdm-migrator-1.0.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/conftest.py` & `invenio-rdm-migrator-1.0.0a6/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,41 +7,52 @@
 
 """Pytest configuration."""
 
 import tempfile
 
 import pytest
 
+from invenio_rdm_migrator.streams.cache import ParentsCache
+
 
 @pytest.fixture(scope="function")
 def tmp_dir():
     """Yields a temporary directory."""
     tmp_dir = tempfile.TemporaryDirectory()
     yield tmp_dir
     tmp_dir.cleanup()
 
 
 @pytest.fixture(scope="module")
-def parent_cache():
+def parents_cache():
     """Records parent cache.
 
     Keys are concept recids and values are UUIDs.
     """
-    return {"123456": "12345678-abcd-1a2b-3c4d-123abc456def"}
+    cache = ParentsCache()
+    cache.add(
+        "123456",
+        {
+            "id": "1234abcd-1234-5678-abcd-123abc456def",
+            "latest_id": "12345678-abcd-1a2b-3c4d-123abc456def",
+            "latest_index": 1,
+        },
+    )
+    return cache
 
 
 @pytest.fixture(scope="module")
 def communities_cache():
     """Communities cache.
 
     Keys are community slugs and values are UUIDs.
     """
     return {"comm": "12345678-abcd-1a2b-3c4d-123abc456def"}
 
 
 @pytest.fixture(scope="module")
-def cache(parent_cache, communities_cache):
+def cache(parents_cache, communities_cache):
     """Global cache containing the other ones."""
     return {
-        "parents": parent_cache,
+        "parents": parents_cache,
         "communities": communities_cache,
     }
```

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # the db queries will be mocked
     load = CommunityCopyLoad(cache, "None", tmp_dir.name)
     yield load
     load._cleanup()
 
 
 @patch(
-    "invenio_rdm_migrator.load.postgresql.uuid4",
+    "invenio_rdm_migrator.load.ids.uuid4",
     lambda: "12345678-abcd-1a2b-3c4d-123abc456def",
 )
 def test_community_load_prepare(community_copy_load, transformed_community_entry):
     """Test the table preparation (file creation)."""
     tables = list(community_copy_load._prepare([transformed_community_entry]))
 
     # assert tables
```

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/communities/test_communities_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/files/conftest.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # the db queries will be mocked
     load = FilesCopyLoad(cache={}, db_uri="None", tmp_dir=tmp_dir.name)
     yield load
     load._cleanup()
 
 
 @patch(
-    "invenio_rdm_migrator.load.postgresql.uuid4",
+    "invenio_rdm_migrator.load.ids.uuid4",
     lambda: "12345678-abcd-1a2b-3c4d-123abc456def",
 )
 def test_files_load_prepare(files_copy_load, transformed_files_entry):
     """Test the table preparation (file creation)."""
     tables = list(files_copy_load._prepare([transformed_files_entry]))
 
     # assert tables
```

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # the db queries will be mocked
     load = RequestCopyLoad(cache, "None", tmp_dir.name)
     yield load
     load._cleanup()
 
 
 @patch(
-    "invenio_rdm_migrator.load.postgresql.uuid4",
+    "invenio_rdm_migrator.load.ids.uuid4",
     lambda: "12345678-abcd-1a2b-3c4d-123abc456def",
 )
 def test_request_load_prepare(request_copy_load, transformed_incl_req_entry):
     """Test the table preparation (file creation)."""
     tables = list(request_copy_load._prepare([transformed_incl_req_entry]))
 
     # assert tables
```

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-1.0.0a6/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

