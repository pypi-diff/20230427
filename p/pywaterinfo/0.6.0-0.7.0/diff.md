# Comparing `tmp/pywaterinfo-0.6.0.tar.gz` & `tmp/pywaterinfo-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pywaterinfo/pywaterinfo/dist/tmp64cuoo9q/pywaterinfo-0.6.0.tar", last modified: Tue Jan 25 23:07:07 2022, max compression
+gzip compressed data, was "pywaterinfo-0.7.0.tar", last modified: Thu Apr 27 14:14:16 2023, max compression
```

## Comparing `pywaterinfo-0.6.0.tar` & `pywaterinfo-0.7.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9290 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/workflows/binder.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.github/workflows/update_docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4842 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     5088 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/docs/_static/img/
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/_static/img/logo_fluves.png
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/_static/img/logo_vito.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/api/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/conduct.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8453 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1160 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/license.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1582 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/timeseriesgroupids.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8927 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/src/pywaterinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/src/pywaterinfo/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    34199 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/src/pywaterinfo/waterinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 23:06:03.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/src/pywaterinfo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 23:07:07.000000 pywaterinfo-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/tests/test_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21530 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/tests/test_waterinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-01-25 23:05:55.000000 pywaterinfo-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.495988 pywaterinfo-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.487988 pywaterinfo-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/workflows/binder.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.github/workflows/update_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-27 14:14:16.495988 pywaterinfo-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5088 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/_static/img/logo_fluves.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/_static/img/logo_vito.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/api/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1386 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/license.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/timeseriesgroupids.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8927 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-27 14:14:16.495988 pywaterinfo-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.487988 pywaterinfo-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/src/pywaterinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/src/pywaterinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/src/pywaterinfo/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36059 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/src/pywaterinfo/waterinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.491988 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-27 14:14:16.000000 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 14:14:16.000000 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:14:16.000000 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:12:55.000000 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-27 14:14:16.000000 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 14:14:16.000000 pywaterinfo-0.7.0/src/pywaterinfo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:14:16.495988 pywaterinfo-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/tests/test_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24425 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/tests/test_waterinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-27 14:12:31.000000 pywaterinfo-0.7.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywaterinfo-0.6.0/.coveragerc` & `pywaterinfo-0.7.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/.github/CODE_OF_CONDUCT.rst` & `pywaterinfo-0.7.0/.github/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/.github/CONTRIBUTING.rst` & `pywaterinfo-0.7.0/.github/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
 `This website`_ is generated with Sphinx_. That means we don't have to
 write any html. Content is pulled together from documentation in the code,
 reStructuredText_ files and the package ``conf.py`` settings. If you
 know your way around *Sphinx*, you can `propose a file change`_ to improve
 documentation. If not, `report an issue`_ and we can point you in the right direction.
 
 .. _This website: https://fluves.github.io/pywaterinfo/
-.. _Sphinx: http://www.sphinx-doc.org/en/master/
-.. _reStructuredText: http://docutils.sourceforge.net/rst.html
+.. _Sphinx: https://www.sphinx-doc.org/en/master/
+.. _reStructuredText: https://docutils.sourceforge.net/rst.html
 .. _propose a file change: https://help.github.com/articles/editing-files-in-another-user-s-repository/
 .. _report an issue: https://github.com/fluves/pywaterinfo/issues/new
 
 **Function documentation**
 
 Functions are described as comments near their code and translated to
 documentation using the  `numpy docstring standard`_. If you want to improve a
@@ -188,24 +188,25 @@
 
 ::
 
     tox
 
 You will receive information on the test status and the test coverage of the unit tests.
 
-In order to run all the tests, you need a HIC token, defined as an environmental variable ``HIC_TOKEN``. When you do
-not have a HIC token, you can ignore the token tests for HIC webservice, be defining to not run the tests
-marked with the `nohictoken` label:
+In order to run all the tests, you need a HIC&VMM token, defined as an environmental variables ``HIC_TOKEN``
+and ``VMM_TOKEN` respectively. When you do not have a HIC token, you can ignore the token tests for HIC webservice,
+be defining to not run the tests marked with the `notoken` label:
 
 ::
 
-    pytest -m 'not nohictoken'
+    pytest -m 'not notoken'
 
 The Github actions CI does have the token stored as a *secret*, so you do not really need a token for local testing, as eventual failures
-will be noticed by the Github Actions CI.
+will be noticed by the Github Actions CI. Although, PRs from forks will not have access to these Github secrets, so these
+tests are ignored when running from fork.
 
 Documentation with sphinx
 --------------------------
 
 Build the documentation locally with Sphinx:
 
 ::
```

### Comparing `pywaterinfo-0.6.0/.github/workflows/ci.yml` & `pywaterinfo-0.7.0/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -13,39 +13,45 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.7, 3.8, 3.9, '3.10', 3.11]
         fail-fast: [false]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .[develop]
+        pip install -e .[develop,cache]
     - name: Run precommit hooks & linting
+      if: matrix.python-version == '3.9'
       run: |
         python -m pip install --upgrade pre-commit
         pre-commit run --all-files
-      if: matrix.python-version == '3.7'
-    - name: Test with pytest
+    - name: Test with pytest when internal PR
+      if: ${{ github.event.pull_request.head.repo.full_name == 'fluves/pywaterinfo' }}
       env:
         HIC_TOKEN: ${{ secrets.HIC_TOKEN }}
         VMM_TOKEN: ${{ secrets.VMM_TOKEN }}
       run: |
         pytest
-    - name: Test with tox
+    - name: Test with pytest when fork PR
+      if: ${{ github.event.pull_request.head.repo.full_name != 'fluves/pywaterinfo' }}
+      run: |
+        pytest -m 'not notoken'
+    - name: Test with tox when internal PR
+      if: ${{ github.event.pull_request.head.repo.full_name == 'fluves/pywaterinfo' }}
       env:
         HIC_TOKEN: ${{ secrets.HIC_TOKEN }}
         VMM_TOKEN: ${{ secrets.VMM_TOKEN }}
       run: |
         tox
     - name: Test doctests
       run: |
```

### Comparing `pywaterinfo-0.6.0/.github/workflows/deploy.yml` & `pywaterinfo-0.7.0/.github/workflows/deploy.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 name: Upload Python Package
-
 on:
   release:
     types: [created]
-
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Get all git tags
       run: git fetch --prune --unshallow --tags
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.7'
+        python-version: '3.9'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .[develop]
+        pip install -e .[develop,cache]
         pip install setuptools wheel twine
     - name: Build documentation
       run: |
         tox -e docs
     - name: Deploy documentation
       uses: peaceiris/actions-gh-pages@v3
       with:
```

### Comparing `pywaterinfo-0.6.0/.github/workflows/update_docs.yml` & `pywaterinfo-0.7.0/.github/workflows/update_docs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 on:
   workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Get all git tags
       run: git fetch --prune --unshallow --tags
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.7'
+        python-version: '3.9'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .[develop]
+        pip install -e .[develop,cache]
     - name: Build documentation
       run: |
         tox -e docs
     - name: Deploy documentation
       uses: peaceiris/actions-gh-pages@v3
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pywaterinfo-0.6.0/.gitignore` & `pywaterinfo-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/.pre-commit-config.yaml` & `pywaterinfo-0.7.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/psf/black
-  rev: 21.12b0
+  rev: 23.1.0
   hooks:
     - id: black
-      language_version: python3.7
+      language_version: python3.9
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.1.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=no']
 
-- repo: https://gitlab.com/pycqa/flake8
-  rev: 3.9.2
+- repo: https://github.com/pycqa/flake8
+  rev: 6.0.0
   hooks:
   - id: flake8
     args: ['--max-line-length=88']  # default of Black
 
 - repo: https://github.com/pre-commit/mirrors-isort
   rev: v5.10.1
   hooks:
```

### Comparing `pywaterinfo-0.6.0/CHANGELOG.rst` & `pywaterinfo-0.7.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+Version 0.7.0
+=============
+
+- Make the caching logic opt-in and deactivated by default (#61).
+- Update the CI setup to support Python 3.10 and 3.11 (#60)
+- Add support for proxies when using pywaterinfo behind a company http proxy (#59, by @stijnvanlooy)
+
 Version 0.6.0
 =============
 
 - Add support for datetime with zoneinfo tzinfo in python 3.9 (#48, by dbkhout)
 - Add citation file using Citation File Format (CFF) (#43)
 
 Version 0.5.1
```

### Comparing `pywaterinfo-0.6.0/CITATION.cff` & `pywaterinfo-0.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/LICENSE` & `pywaterinfo-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/PKG-INFO` & `pywaterinfo-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: pywaterinfo
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package to download time series data from waterinfo.be
 Home-page: https://github.com/fluves/pywaterinfo
 Author: Stijn Van Hoey
 Author-email: stijn@fluves.com
 License: mit
 Project-URL: Documentation, https://github.com/fluves/pywaterinfo
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: cache
 Provides-Extra: develop
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # pywaterinfo
 
 Python package to download time series data from waterinfo.be
@@ -110,9 +113,7 @@
 
 * We welcome [contributions](.github/CONTRIBUTING.rst) including bug reports.
 * License: MIT
 * Please note that this project is released with a [Contributor Code of Conduct](.github/CODE_OF_CONDUCT.rst). By participating in this project you agree to abide by its terms.
 
 This project has been set up using PyScaffold 3.2.3. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
-
-
```

### Comparing `pywaterinfo-0.6.0/README.md` & `pywaterinfo-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/README.rst` & `pywaterinfo-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/Makefile` & `pywaterinfo-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/_static/img/logo_fluves.png` & `pywaterinfo-0.7.0/docs/_static/img/logo_fluves.png`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/_static/img/logo_vito.png` & `pywaterinfo-0.7.0/docs/_static/img/logo_vito.png`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/conf.py` & `pywaterinfo-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/index.rst` & `pywaterinfo-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/installation.rst` & `pywaterinfo-0.7.0/docs/installation.rst`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 
 The package releases are available on `Pypi <https://pypi.org/>`_. To install the package:
 
 ::
 
     pip install pywaterinfo
 
+To use caching to overcome redundant requests to the waterinfo APi, install the cache dependencies:
+
+::
+
+    pip install pywaterinfo[cache]
+
+See :ref:`cache` documentation for more information on the caching feature.
+
 
 Using setuptools
 ----------------
 
 After downloading the code from the repository, e.g. using `git`:
 
 ::
```

### Comparing `pywaterinfo-0.6.0/docs/logging.rst` & `pywaterinfo-0.7.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/docs/timeseriesgroupids.rst` & `pywaterinfo-0.7.0/docs/timeseriesgroupids.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
       afvoer, uur, 192892, discharge, hour
       afvoer, dag, 192893, discharge, day
       afvoer, maand, 192894, discharge, month
       afvoer, jaar, 192895, discharge, year
       bodem_verzadiging, 15min, 192929, soil_saturation, 15min
       bodem_vocht, 15min, 192928, soil_moisture, 15min
       dauwpunt_temperatuur, 15min, 192923, dew_point_temperature, 15min
+      geleidbaarheid (permanent meetnet), 15min, 383065, conductivity (continuous network), 15min
+      geleidbaarheid (project), 15min, 381863, conductivity (project based), 15min
       grondtemperatuur, 15min, 192924, ground_temperature, 15min
       grondwarmte, 15min, 192916, ground_heat, 15min
       instraling, 15min, 192920, irradiance, 15min
       luchtdruk, 15min, 192918, air_pressure, 15min
       luchttemperatuur175cm, 15min, 192922, air_temperature_175cm, 15min
       neerslag, 1m, 199792, rainfall, 1min
       neerslag, 15min, 192896, rainfall, 15min
```

### Comparing `pywaterinfo-0.6.0/docs/tutorial.rst` & `pywaterinfo-0.7.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/setup.cfg` & `pywaterinfo-0.7.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -12,40 +12,42 @@
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	pandas
 	requests
-	requests-cache>=0.8
 python_requires = >=3.7
 
 [options.package_data]
 pywaterinfo = data/*
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
+cache = requests-cache>=0.8
 develop = 
 	tox
 	flake8
 	pytest
 	pytest-cov
 	sphinx
 	sphinx_rtd_theme
@@ -65,15 +67,15 @@
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 markers = 
-	nohictoken: marks tests relying on HIC token (deselect with '-m "not nohictoken"')
+	notoken: marks tests relying on HIC/VMM token (deselect with '-m "not notoken"')
 
 [aliases]
 dists = bdist_wheel
 
 [bdist_wheel]
 universal = 1
```

### Comparing `pywaterinfo-0.6.0/setup.py` & `pywaterinfo-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/src/pywaterinfo/__init__.py` & `pywaterinfo-0.7.0/src/pywaterinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/src/pywaterinfo/utils.py` & `pywaterinfo-0.7.0/src/pywaterinfo/utils.py`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/src/pywaterinfo/waterinfo.py` & `pywaterinfo-0.7.0/src/pywaterinfo/waterinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 
 import datetime
 import logging
 import pandas as pd
 import pytz
 import re
 import requests
-import requests_cache
+
+try:
+    import requests_cache
+
+    request_cache_support = True
+except ImportError:
+    request_cache_support = False
+
 
 """
 INFO:
 
 https://download.waterinfo.be/tsmdownload/KiWIS/KiWIS?service=kisters& \
     type=QueryServices&format=html&request=getrequestinfo
 other KIWIS-python clients:
@@ -43,46 +50,79 @@
 class WaterinfoException(Exception):
     """Raised when the Waterinfo data request inputs are wrong"""
 
     pass
 
 
 class Waterinfo:
-    def __init__(self, provider: str = "vmm", token: str = None):
+    def __init__(
+        self,
+        provider: str = "vmm",
+        token: str = None,
+        proxies: dict = None,
+        cache: bool = False,
+    ):
         """Request data from waterinfo.be
 
         Parameters
         ----------
         provider : vmm | hic
             Define the origin of the data on waterinfo you're looking for. Either
             provided by VMM (vmm) or HIC (hic)
         token : str
             Token as provided by VMM on project-level.
+        proxies: dict
+            Dictionary mapping protocol or protocol and host to the URL of the proxy
+            (e.g. {‘http’: ‘foo.bar:3128’, ‘http://host.name’: ‘foo.bar:4012’}) to be
+            used on each Request
+        cache : bool, default False
+            If True, a cached session is used to make sure consecutive calls for the
+            same data are stored in a local cache.
         """
 
+        # TODO - add info on missing installation of requests-cache
+
         # set the base string linked to the data provider
         if provider == "vmm":
             self._base_url = VMM_BASE
             self._auth_url = VMM_AUTH
             self._datasource = "1"
         elif provider == "hic":
             self._base_url = HIC_BASE
             self._auth_url = HIC_AUTH
             self._datasource = "4"
         else:
             raise WaterinfoException("Provider is either 'vmm' or 'hic'.")
 
         # Use requests-cache session
-        self._request = requests_cache.CachedSession(
-            cache_name="pywaterinfo_cache.sqlite",
-            backend="sqlite",
-            expire_after=CACHE_RETENTION,
-            stale_if_error=False,
-            use_temp=True,
-        )
+        if cache:
+            if request_cache_support:
+                self._cache = True
+                self._request = requests_cache.CachedSession(
+                    cache_name="pywaterinfo_cache.sqlite",
+                    use_memory=False,
+                    cache_control=True,
+                    expire_after=CACHE_RETENTION,
+                    stale_if_error=False,
+                    use_cache_dir=True,
+                    proxies=proxies,
+                )
+            else:
+                raise Exception(
+                    "The required packages to support caching are not "
+                    "installed. Install them with "
+                    "`pip install pywaterinfo[cache]`."
+                )
+        else:
+            self._cache = False
+            self._request = requests.Session()
+            if proxies:
+                self._request.proxies.update(proxies)
+
+        self._proxies = proxies
 
         self.__default_args = {
             "service": "kisters",
             "type": "QueryServices",
             "format": "json",
             "datasource": self._datasource,
             "timezone": "UTC",
@@ -96,14 +136,15 @@
                 headers={
                     "Authorization": f"Basic {token}",
                     "scope": "none",
                     "Content-Type": "application/x-www-form-urlencoded",
                     "charset": "UTF-8",
                 },
                 data={"grant_type": "client_credentials"},
+                proxies=proxies,
             )
             res.raise_for_status()
             res_parsed = res.json()
             self._token_header = {
                 "Authorization": f"{res_parsed['token_type']} "
                 f"{res_parsed['access_token']}"
             }
@@ -122,22 +163,24 @@
         info, _ = self.request_kiwis(query_param, headers=headers)
         self._kiwis_info = info[0]["Requests"]
 
         self._default_params = ["format", "returnfields", "request"]
 
         # clean up cache old entries (requests-cache only removes/updates
         # entries that are reused, so this remove piling too much cache.)
-        self._request.remove_expired_responses(CACHE_RETENTION)
+        if cache:
+            self._request.cache.delete(expired=True)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} object, " f"Query from {self._base_url!r}>"
 
     def clear_cache(self):
         """Clean up the cache."""
-        self._request.cache.clear()
+        if self._cache:
+            self._request.cache.clear()
 
     def request_kiwis(self, query: dict, headers: dict = None) -> dict:
         """http call to waterinfo.be KIWIS API
 
         General call used to request information and data from waterinfo.be, providing
         error handling and json parsing. The service, type, format (json),
         datasource and timezone (UTC) are provided by default (but can be overridden
@@ -161,15 +204,15 @@
         Examples
         --------
         >>> from pywaterinfo import Waterinfo
         >>> vmm = Waterinfo("vmm")
         >>> # get the API info/documentation from kiwis
         >>> data, res = vmm.request_kiwis({"request": "getRequestInfo"})
         >>> data        #doctest: +ELLIPSIS
-        [{'Title': 'KISTERS QueryServices - Request Inform...file'}}}}}}]
+        [{'Title': 'KISTERS QueryServices - Request Inform...}}}}}]
         >>> res.status_code
         200
         >>> # get the timeseries data from last day from time series 78124042
         >>> data, res = vmm.request_kiwis({"request": "getTimeseriesValues",
         ...                                "ts_id": "78124042",
         ...                                "period": "P1D"})
         >>> data        #doctest: +ELLIPSIS
@@ -199,26 +242,37 @@
             if key not in query.keys()
         }
         query.update(defaults)
         if not headers:
             headers = dict()
         if self._token_header:
             headers.update(self._token_header)
-        res = self._request.get(self._base_url, params=query, headers=headers)
+        res = self._request.get(
+            self._base_url, params=query, headers=headers, proxies=self._proxies
+        )
 
         if res.status_code != requests.codes.ok:
             raise KiwisException(
-                f"Waterinfo call returned {res.status_code} error"
+                f"Waterinfo call returned {res.status_code} error "
                 f"with the message {res.content}"
             )
 
-        if res.from_cache:
-            logging.info(f"Request {res.url} reused from cache.")
+        if self._cache:
+            if res.from_cache:
+                logging.info(f"Request {res.url} reused from cache.")
+            else:
+                logging.info(
+                    f"Successful waterinfo API request with call {res.url} "
+                    f"(call to waterinfo.be with cache activated)."
+                )
         else:
-            logging.info(f"Successful waterinfo API request with call {res.url}")
+            logging.info(
+                f"Successful waterinfo API request with call {res.url} "
+                f"(call to waterinfo.be with without cache activated)."
+            )
 
         parsed = res.json()
         if (
             type(parsed) is dict
             and "type" in parsed.keys()
             and parsed["type"] == "error"
         ):
@@ -241,15 +295,15 @@
         if "Optionalfields" in self._kiwis_info[request]:
             optional_parameters = set(
                 self._kiwis_info[request]["Optionalfields"]["Content"].keys()
             )
         else:
             optional_parameters = set()
 
-        for (parameter, _) in query.items():
+        for parameter, _ in query.items():
             if parameter not in (
                 supported_parameters | optional_parameters | set(self._default_params)
             ):
                 raise WaterinfoException(
                     f"Parameter '{parameter}' not in requestInfo for {request}. Check "
                     f"{self._base_url}?service=kisters&type=queryServices"
                     f"&request=getRequestInfo "
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pywaterinfo-0.6.0/src/pywaterinfo.egg-info/PKG-INFO` & `pywaterinfo-0.7.0/src/pywaterinfo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: pywaterinfo
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package to download time series data from waterinfo.be
 Home-page: https://github.com/fluves/pywaterinfo
 Author: Stijn Van Hoey
 Author-email: stijn@fluves.com
 License: mit
 Project-URL: Documentation, https://github.com/fluves/pywaterinfo
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: cache
 Provides-Extra: develop
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # pywaterinfo
 
 Python package to download time series data from waterinfo.be
@@ -110,9 +113,7 @@
 
 * We welcome [contributions](.github/CONTRIBUTING.rst) including bug reports.
 * License: MIT
 * Please note that this project is released with a [Contributor Code of Conduct](.github/CODE_OF_CONDUCT.rst). By participating in this project you agree to abide by its terms.
 
 This project has been set up using PyScaffold 3.2.3. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
-
-
```

### Comparing `pywaterinfo-0.6.0/src/pywaterinfo.egg-info/SOURCES.txt` & `pywaterinfo-0.7.0/src/pywaterinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywaterinfo-0.6.0/tests/conftest.py` & `pywaterinfo-0.7.0/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,19 +26,38 @@
 
 @pytest.fixture(scope="module")
 def vmm_connection():
     return Waterinfo("vmm", token=vmm_client)
 
 
 @pytest.fixture(scope="module")
+def vmm_cached_connection():
+    session = Waterinfo("vmm", token=vmm_client, cache=True)
+    session.clear_cache()
+    return session
+
+
+@pytest.fixture(scope="module")
 def hic_connection():
     if hic_client:
         return Waterinfo("hic", token=hic_client)
     else:
         return Waterinfo("hic")
 
 
 @pytest.fixture(scope="module")
+def hic_cached_connection():
+    if hic_client:
+        session = Waterinfo("hic", token=hic_client, cache=True)
+        session.clear_cache()
+        return session
+    else:
+        session = Waterinfo("hic", cache=True)
+        session.clear_cache()
+        return session
+
+
+@pytest.fixture(scope="module")
 def df_timeseries(vmm_connection):
     return vmm_connection.get_timeseries_values(
         78124042, start="20190501", end="20190502"
     )
```

### Comparing `pywaterinfo-0.6.0/tests/test_cache.py` & `pywaterinfo-0.7.0/tests/test_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import time
 
 from pywaterinfo import Waterinfo
 
 
-def test_cache_vmm(vmm_connection):
+def test_cache_vmm(vmm_cached_connection):
     """Second call of the same request is retrieved from cache for VMM requests."""
-    vmm_connection.clear_cache()
-    data, res = vmm_connection.request_kiwis({"request": "getRequestInfo"})
+    vmm_cached_connection.clear_cache()
+    data, res = vmm_cached_connection.request_kiwis({"request": "getRequestInfo"})
     assert not res.from_cache
-    data, res = vmm_connection.request_kiwis({"request": "getRequestInfo"})
+    data, res = vmm_cached_connection.request_kiwis({"request": "getRequestInfo"})
     assert res.from_cache
 
 
-def test_cache_hic(hic_connection):
+def test_cache_hic(hic_cached_connection):
     """Second call of the same request is retrieved from cache for HIC requests."""
-    hic_connection.clear_cache()
-    data, res = hic_connection.request_kiwis(
+    hic_cached_connection.clear_cache()
+    # patch/exclude cache control to use retention time only
+    hic_cached_connection._request.settings.cache_control = False
+    data, res = hic_cached_connection.request_kiwis(
         query={"request": "getTimeseriesValueLayer", "timeseriesgroup_id": "156207"}
     )
     assert not res.from_cache
-    data, res = hic_connection.request_kiwis(
+    data, res = hic_cached_connection.request_kiwis(
         query={"request": "getTimeseriesValueLayer", "timeseriesgroup_id": "156207"}
     )
     assert res.from_cache
 
 
 {"request": "getTimeseriesValueLayer", "timeseriesgroup_id": "156207"}
 
 
-def test_clear_cache(vmm_connection):
+def test_clear_cache(vmm_cached_connection):
     """Cache is cleared."""
-    vmm_connection.clear_cache()
-    data, res = vmm_connection.request_kiwis({"request": "getRequestInfo"})
+    data, res = vmm_cached_connection.request_kiwis({"request": "getRequestInfo"})
     assert not res.from_cache
-    vmm_connection.clear_cache()
-    data, res = vmm_connection.request_kiwis({"request": "getRequestInfo"})
+    vmm_cached_connection.clear_cache()
+    data, res = vmm_cached_connection.request_kiwis({"request": "getRequestInfo"})
     assert not res.from_cache
 
 
 def test_cache_retention_between_sessions():
-    """Requests are chached in between two sessions."""
-    vmm = Waterinfo("vmm")
+    """Requests are cached in between two sessions."""
+    vmm = Waterinfo("vmm", cache=True)
     vmm.clear_cache()
     _, res = vmm.request_kiwis({"request": "getRequestInfo"})
     assert not res.from_cache
 
     # New session reuses the same database
-    vmm = Waterinfo("vmm")
+    vmm = Waterinfo("vmm", cache=True)
     _, res = vmm.request_kiwis({"request": "getRequestInfo"})
     assert res.from_cache
 
 
 def test_cache_retention(patch_retention):
     """Request is not from cache after expiration date.
 
@@ -60,20 +61,22 @@
     -----
     See requests-cache.readthedocs.io/en/stable/user_guide/headers.html,
     conditional requests are automatically sent for any servers that support them. Once
     a cached response expires, it will only be updated if the
     remote content has changed. Hence, we check here for expiration first, remove the
     expired cache and check for `from_cache` in a new request.
     """
-    vmm = Waterinfo("vmm")
+    vmm = Waterinfo("vmm", cache=True)
+    # patch/exclude cache control to use retention time only
+    vmm._request.settings.cache_control = False
     vmm.clear_cache()
     _, res = vmm.request_kiwis({"request": "getRequestInfo"})
     assert not res.from_cache
 
     time.sleep(1)
-    vmm = Waterinfo("vmm")
+    vmm._request.cache
     _, res = vmm.request_kiwis({"request": "getRequestInfo"})
     assert res.is_expired
 
-    vmm._request.remove_expired_responses()
+    vmm._request.cache.delete(expired=True)
     _, res = vmm.request_kiwis({"request": "getRequestInfo"})
     assert not res.from_cache
```

### Comparing `pywaterinfo-0.6.0/tox.ini` & `pywaterinfo-0.7.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 # THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [main]
 name = pywaterinfo
 
 [tox]
 minversion = 3.15
-envlist = py37,py38,py39
+envlist = py{37,38,39,310,311}
 skip_missing_interpreters=true
 
 
 [testenv]
 description = invoke pytest to run automated tests
 allowlist_externals = pytest
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
-    HOME HIC_TOKEN VMM_TOKEN
+    HOME
+    HIC_TOKEN
+    VMM_TOKEN
 extras =
+    cache
     develop
 commands =
     pytest {posargs}
 
 
 [testenv:{clean,build}]
 description =
@@ -46,14 +49,15 @@
 setenv =
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
 extras =
     develop
+    cache
 commands =
     sphinx-build -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
 
 [testenv:pre-commit]
 skip_install = true
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
@@ -61,12 +65,13 @@
 
 [testenv:dev]
 description = Create development environment with venv and register ipykernel
 basepython = python3
 usedevelop = true
 envdir = {toxinidir}/venv
 extras =
+    cache
     develop
 deps =
     ipykernel
 commands =
     python -m ipykernel install --user --name {[main]name} --display-name 'Python py39 ({[main]name})'
```

