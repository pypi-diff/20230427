# Comparing `tmp/wmflib-1.2.1.tar.gz` & `tmp/wmflib-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmflib-1.2.1.tar", last modified: Thu Feb  2 16:10:48 2023, max compression
+gzip compressed data, was "wmflib-1.2.2.tar", last modified: Thu Apr 27 16:58:20 2023, max compression
```

## Comparing `wmflib-1.2.1.tar` & `wmflib-1.2.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.325195 wmflib-1.2.1/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2020-10-23 09:48:59.000000 wmflib-1.2.1/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)      153 2021-02-18 16:38:06.000000 wmflib-1.2.1/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       95 2020-10-23 09:48:59.000000 wmflib-1.2.1/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      204 2023-02-02 15:29:16.000000 wmflib-1.2.1/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)    12091 2023-02-02 15:29:16.000000 wmflib-1.2.1/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.1/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    35148 2020-10-23 09:48:59.000000 wmflib-1.2.1/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-02-02 16:10:48.325486 wmflib-1.2.1/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      567 2021-01-04 11:44:13.000000 wmflib-1.2.1/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.168111 wmflib-1.2.1/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      608 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.175113 wmflib-1.2.1/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.176380 wmflib-1.2.1/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/source/_static/themes_override.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.195272 wmflib-1.2.1/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)      381 2021-11-11 14:12:19.000000 wmflib-1.2.1/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-10-23 09:49:17.000000 wmflib-1.2.1/doc/source/api/wmflib.actions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2020-10-23 09:49:17.000000 wmflib-1.2.1/doc/source/api/wmflib.config.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-12-21 17:56:39.000000 wmflib-1.2.1/doc/source/api/wmflib.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      129 2021-01-04 11:44:13.000000 wmflib-1.2.1/doc/source/api/wmflib.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       36 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/source/api/wmflib.dns.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/source/api/wmflib.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-02-18 16:38:06.000000 wmflib-1.2.1/doc/source/api/wmflib.fileio.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       36 2021-07-14 07:59:46.000000 wmflib-1.2.1/doc/source/api/wmflib.idm.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-12-21 17:56:39.000000 wmflib-1.2.1/doc/source/api/wmflib.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       77 2021-01-04 11:44:13.000000 wmflib-1.2.1/doc/source/api/wmflib.irc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-10-23 09:49:17.000000 wmflib-1.2.1/doc/source/api/wmflib.phabricator.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-12-21 17:56:39.000000 wmflib-1.2.1/doc/source/api/wmflib.prometheus.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2020-11-02 11:43:53.000000 wmflib-1.2.1/doc/source/api/wmflib.requests.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     8012 2023-02-02 15:29:16.000000 wmflib-1.2.1/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1160 2021-11-11 14:12:19.000000 wmflib-1.2.1/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       58 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       61 2020-10-23 09:48:59.000000 wmflib-1.2.1/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1670 2022-03-09 19:50:10.000000 wmflib-1.2.1/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2023-02-02 16:10:48.327444 wmflib-1.2.1/setup.cfg
--rw-r--r--   0 riccardo   (501) staff       (20)     2548 2023-02-02 15:29:16.000000 wmflib-1.2.1/setup.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1762 2023-02-02 15:29:16.000000 wmflib-1.2.1/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.228930 wmflib-1.2.1/wmflib/
--rw-r--r--   0 riccardo   (501) staff       (20)      395 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5894 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/actions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1796 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/config.py
--rw-r--r--   0 riccardo   (501) staff       (20)      578 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11577 2022-02-14 11:47:28.000000 wmflib-1.2.1/wmflib/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8271 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/dns.py
--rw-r--r--   0 riccardo   (501) staff       (20)      532 2020-10-23 09:48:59.000000 wmflib-1.2.1/wmflib/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2524 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/fileio.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4482 2021-08-04 08:43:52.000000 wmflib-1.2.1/wmflib/idm.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10205 2023-02-02 15:29:16.000000 wmflib-1.2.1/wmflib/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2929 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/irc.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3741 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/phabricator.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6563 2023-02-02 15:29:16.000000 wmflib-1.2.1/wmflib/prometheus.py
--rw-r--r--   0 riccardo   (501) staff       (20)       65 2021-01-04 11:44:13.000000 wmflib-1.2.1/wmflib/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)     7270 2023-02-02 15:29:16.000000 wmflib-1.2.1/wmflib/requests.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.260096 wmflib-1.2.1/wmflib/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)     1062 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.155560 wmflib-1.2.1/wmflib/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.272504 wmflib-1.2.1/wmflib/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       20 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/config/config.ini
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/config/empty.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       28 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/config/invalid.ini
--rw-r--r--   0 riccardo   (501) staff       (20)       41 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/config/invalid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/config/valid.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.286585 wmflib-1.2.1/wmflib/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/phabricator/invalid.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/fixtures/phabricator/valid.conf
--rw-r--r--   0 riccardo   (501) staff       (20)     2211 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.324496 wmflib-1.2.1/wmflib/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       37 2020-10-23 09:48:59.000000 wmflib-1.2.1/wmflib/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      421 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/unit/conftest.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3214 2020-12-21 12:21:13.000000 wmflib-1.2.1/wmflib/tests/unit/test_actions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2483 2020-12-21 12:21:19.000000 wmflib-1.2.1/wmflib/tests/unit/test_config.py
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/unit/test_constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7464 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8326 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/unit/test_dns.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1456 2021-11-11 14:12:19.000000 wmflib-1.2.1/wmflib/tests/unit/test_fileio.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3280 2021-08-04 08:43:52.000000 wmflib-1.2.1/wmflib/tests/unit/test_idm.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12913 2023-02-02 15:29:16.000000 wmflib-1.2.1/wmflib/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1660 2021-02-18 16:38:06.000000 wmflib-1.2.1/wmflib/tests/unit/test_irc.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3362 2020-10-23 09:49:17.000000 wmflib-1.2.1/wmflib/tests/unit/test_phabricator.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3416 2022-04-04 10:17:39.000000 wmflib-1.2.1/wmflib/tests/unit/test_prometheus.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3964 2023-02-02 15:29:16.000000 wmflib-1.2.1/wmflib/tests/unit/test_requests.py
--rw-r--r--   0 riccardo   (501) staff       (20)      474 2023-02-02 15:29:16.000000 wmflib-1.2.1/wmflib/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-02-02 16:10:48.255960 wmflib-1.2.1/wmflib.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-02-02 16:10:47.000000 wmflib-1.2.1/wmflib.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     2083 2023-02-02 16:10:48.000000 wmflib-1.2.1/wmflib.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-02-02 16:10:47.000000 wmflib-1.2.1/wmflib.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-02-02 16:10:47.000000 wmflib-1.2.1/wmflib.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      391 2023-02-02 16:10:47.000000 wmflib-1.2.1/wmflib.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        7 2023-02-02 16:10:47.000000 wmflib-1.2.1/wmflib.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.482677 wmflib-1.2.2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2020-10-23 09:48:59.000000 wmflib-1.2.2/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)      153 2021-02-18 16:38:06.000000 wmflib-1.2.2/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       95 2020-10-23 09:48:59.000000 wmflib-1.2.2/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      204 2023-02-02 15:29:16.000000 wmflib-1.2.2/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)    12694 2023-04-27 16:27:56.000000 wmflib-1.2.2/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.2/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    35148 2020-10-23 09:48:59.000000 wmflib-1.2.2/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-04-27 16:58:20.483047 wmflib-1.2.2/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      567 2021-01-04 11:44:13.000000 wmflib-1.2.2/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.331493 wmflib-1.2.2/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      608 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.351631 wmflib-1.2.2/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.353190 wmflib-1.2.2/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/_static/themes_override.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.385903 wmflib-1.2.2/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)      381 2021-11-11 14:12:19.000000 wmflib-1.2.2/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-10-23 09:49:17.000000 wmflib-1.2.2/doc/source/api/wmflib.actions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2020-10-23 09:49:17.000000 wmflib-1.2.2/doc/source/api/wmflib.config.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-12-21 17:56:39.000000 wmflib-1.2.2/doc/source/api/wmflib.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      129 2021-01-04 11:44:13.000000 wmflib-1.2.2/doc/source/api/wmflib.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       36 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/api/wmflib.dns.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/api/wmflib.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-02-18 16:38:06.000000 wmflib-1.2.2/doc/source/api/wmflib.fileio.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       36 2021-07-14 07:59:46.000000 wmflib-1.2.2/doc/source/api/wmflib.idm.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-12-21 17:56:39.000000 wmflib-1.2.2/doc/source/api/wmflib.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       77 2021-01-04 11:44:13.000000 wmflib-1.2.2/doc/source/api/wmflib.irc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-10-23 09:49:17.000000 wmflib-1.2.2/doc/source/api/wmflib.phabricator.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-12-21 17:56:39.000000 wmflib-1.2.2/doc/source/api/wmflib.prometheus.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2020-11-02 11:43:53.000000 wmflib-1.2.2/doc/source/api/wmflib.requests.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     8012 2023-02-02 15:29:16.000000 wmflib-1.2.2/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1160 2021-11-11 14:12:19.000000 wmflib-1.2.2/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       58 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       61 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1670 2022-03-09 19:50:10.000000 wmflib-1.2.2/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2023-04-27 16:58:20.484525 wmflib-1.2.2/setup.cfg
+-rw-r--r--   0 riccardo   (501) staff       (20)     2491 2023-04-27 16:27:56.000000 wmflib-1.2.2/setup.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1767 2023-04-27 16:27:56.000000 wmflib-1.2.2/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.422803 wmflib-1.2.2/wmflib/
+-rw-r--r--   0 riccardo   (501) staff       (20)      395 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5894 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/actions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1796 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/config.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      578 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11577 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8282 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/dns.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      532 2020-10-23 09:48:59.000000 wmflib-1.2.2/wmflib/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2524 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/fileio.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4482 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/idm.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10205 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2929 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/irc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3741 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/phabricator.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6563 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/prometheus.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       65 2021-01-04 11:44:13.000000 wmflib-1.2.2/wmflib/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)     7270 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/requests.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.433593 wmflib-1.2.2/wmflib/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1062 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.313361 wmflib-1.2.2/wmflib/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.450248 wmflib-1.2.2/wmflib/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       20 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/config.ini
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/empty.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       28 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/invalid.ini
+-rw-r--r--   0 riccardo   (501) staff       (20)       41 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/invalid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/valid.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.452334 wmflib-1.2.2/wmflib/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/phabricator/invalid.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/phabricator/valid.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)     2211 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.481687 wmflib-1.2.2/wmflib/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       37 2020-10-23 09:48:59.000000 wmflib-1.2.2/wmflib/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      421 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/conftest.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3214 2020-12-21 12:21:13.000000 wmflib-1.2.2/wmflib/tests/unit/test_actions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2483 2020-12-21 12:21:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_config.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7464 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8332 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/tests/unit/test_dns.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1456 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_fileio.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3280 2021-08-04 08:43:52.000000 wmflib-1.2.2/wmflib/tests/unit/test_idm.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12913 2023-02-02 15:29:16.000000 wmflib-1.2.2/wmflib/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1660 2021-02-18 16:38:06.000000 wmflib-1.2.2/wmflib/tests/unit/test_irc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3362 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/unit/test_phabricator.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3416 2022-04-04 10:17:39.000000 wmflib-1.2.2/wmflib/tests/unit/test_prometheus.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3964 2023-02-02 15:29:16.000000 wmflib-1.2.2/wmflib/tests/unit/test_requests.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      474 2023-02-02 15:29:16.000000 wmflib-1.2.2/wmflib/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.429893 wmflib-1.2.2/wmflib.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     2083 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        7 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/top_level.txt
```

### Comparing `wmflib-1.2.1/CHANGELOG.rst` & `wmflib-1.2.2/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 wmflib Changelog
 ----------------
 
+`v1.2.2`_ (2023-04-27)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Bug fixes
+"""""""""
+
+* dns: clarify the type of the ``nameserver_addresses`` argument of the Dns class to adhere to the dnspython one.
+* dns: convert the sequence of ``nameserver_addresses`` to list to adhere to what dnspython is expecting.
+* requests: rename the type alias ``TypeTimeout`` to ``TimeoutType`` to adhere to pylint naming formats.
+
+Miscellanea
+"""""""""""
+
+* tox: disable bandit's ``request_without_timeout`` check in tests due to false positives.
+
 `v1.2.1`_ (2023-02-02)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Minor improvements
 """"""""""""""""""
 
 * interactive: log the response to ``ask_input`` for easier troubleshooting. Indirectly logs also the response to
@@ -331,7 +346,8 @@
 .. _`v1.0.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.0.1
 .. _`v1.0.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.0.2
 .. _`v1.1.0`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.0
 .. _`v1.1.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.1
 .. _`v1.1.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.2
 .. _`v1.2.0`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.0
 .. _`v1.2.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.1
+.. _`v1.2.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.2
```

### Comparing `wmflib-1.2.1/LICENSE` & `wmflib-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/PKG-INFO` & `wmflib-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmflib
-Version: 1.2.1
+Version: 1.2.2
 Summary: Generic library for common tasks in the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-pywmflib
 Author: Luca Toscano
 Author-email: ltoscano@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation
 Platform: GNU/Linux
```

### Comparing `wmflib-1.2.1/README.rst` & `wmflib-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/doc/Makefile` & `wmflib-1.2.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/doc/source/conf.py` & `wmflib-1.2.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/doc/source/installation.rst` & `wmflib-1.2.2/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/prospector.yaml` & `wmflib-1.2.2/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/setup.cfg` & `wmflib-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/setup.py` & `wmflib-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open('README.rst', 'r') as readme:
     LONG_DESCRIPTION = readme.read()
 
 
 INSTALL_REQUIRES = [
-    "dnspython>=1.15.0,<2.2.0",  # Temporary upper limit to prevent mypy failures
+    "dnspython>=1.15.0",
     'pyyaml>=3.11',
     'phabricator>=0.7.0',
     'requests',
 ]
 
 # Extra dependencies
 EXTRAS_REQUIRE = {
```

### Comparing `wmflib-1.2.1/tox.ini` & `wmflib-1.2.2/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     flake8: flake8 setup.py wmflib
     unit: py.test --strict-markers --cov-report=term-missing --cov=wmflib wmflib/tests/unit {posargs}
     # Skip some bandit issues:
     # - assert_used (B101) in tests
     # - blacklist of 'input' (B322, for Py2 only) and 'subprocess' (B404) modules
     # - use of subprocess_without_shell_equals_true (B603) to alert if shell True is used instead
     bandit: bandit -l -i -r --skip B404,B603 --exclude './wmflib/tests' ./wmflib/
-    bandit: bandit -l -i -r --skip B101,B404 wmflib/tests
+    bandit: bandit -l -i -r --skip B101,B113,B404 wmflib/tests
     mypy: mypy wmflib/
     prospector: prospector --no-external-config --profile '{toxinidir}/prospector.yaml' {posargs} {toxinidir}
     sphinx: python wmflib/tests/sphinx_checker.py '{toxinidir}'
     sphinx: python setup.py build_sphinx -W -b html
 deps =
     # Use install_requires and the additional extras_require[tests/prospector] from setup.py
     prospector: .[prospector]
```

### Comparing `wmflib-1.2.1/wmflib/actions.py` & `wmflib-1.2.2/wmflib/actions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/config.py` & `wmflib-1.2.2/wmflib/config.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/constants.py` & `wmflib-1.2.2/wmflib/constants.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/decorators.py` & `wmflib-1.2.2/wmflib/decorators.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/dns.py` & `wmflib-1.2.2/wmflib/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     One or more resource records might exist for this domain but no record matches the resource record type requested.
     """
 
 
 class Dns:
     """Class to interact with the DNS."""
 
-    def __init__(self, *, nameserver_addresses: Optional[Sequence] = None, port: Optional[int] = None) -> None:
+    def __init__(self, *, nameserver_addresses: Optional[Sequence[str]] = None, port: Optional[int] = None) -> None:
         """Initialize the instance optionally specifying the nameservers to use.
 
         Examples:
             Using the host's default DNS resolvers::
 
                 >>> from wmflib.dns import Dns
                 >>> dns = Dns()
@@ -49,15 +49,15 @@
                 the default 53. This applies only if a nameserveres is explicitelyes specified.
 
         """
         if nameserver_addresses is not None:
             self._resolver = resolver.Resolver(configure=False)
             if port is not None:
                 self._resolver.port = port
-            self._resolver.nameservers = nameserver_addresses
+            self._resolver.nameservers = list(nameserver_addresses)
         else:
             self._resolver = resolver.Resolver()
 
     def resolve_ipv4(self, name: str) -> List[str]:
         """Perform a DNS lookup for an A record for the given name.
 
         Examples:
```

### Comparing `wmflib-1.2.1/wmflib/exceptions.py` & `wmflib-1.2.2/wmflib/exceptions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/fileio.py` & `wmflib-1.2.2/wmflib/fileio.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/idm.py` & `wmflib-1.2.2/wmflib/idm.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/interactive.py` & `wmflib-1.2.2/wmflib/interactive.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/irc.py` & `wmflib-1.2.2/wmflib/irc.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/phabricator.py` & `wmflib-1.2.2/wmflib/phabricator.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/prometheus.py` & `wmflib-1.2.2/wmflib/prometheus.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Dict, List
 
 import requests
 
 from wmflib.constants import ALL_DATACENTERS
 from wmflib.exceptions import WmflibError
-from wmflib.requests import http_session, TypeTimeout
+from wmflib.requests import http_session, TimeoutType
 
 logger = logging.getLogger(__name__)
 
 
 class PrometheusError(WmflibError):
     """Custom exception class for errors of this module."""
 
@@ -20,21 +20,21 @@
 class PrometheusBase:
     """Base class to interact with Prometheus-like APIs."""
 
     def __init__(self) -> None:
         """Initialize the instance."""
         self._http_session = http_session('.'.join((self.__module__, self.__class__.__name__)))
 
-    def _query(self, url: str, params: Dict[str, str], timeout: TypeTimeout) -> List[Dict]:
+    def _query(self, url: str, params: Dict[str, str], timeout: TimeoutType) -> List[Dict]:
         """Perform a generic query.
 
         Arguments:
             url (str): the URL to query.
             params (dict): a dictionary of the GET parameters to pass to the URL.
-            timeout (:py:data:`wmflib.requests.TypeTimeout`): How many seconds to wait for prometheus to reply before
+            timeout (:py:data:`wmflib.requests.TimeoutType`): How many seconds to wait for prometheus to reply before
                 giving up. This is passed directly to the requests library.
 
         Returns:
             list: returns an empty list if there are no results otherwise return a list of results of the form:
             ``{'metric': {}, 'value': [$timestamp, $value]}``.
 
         Raises:
@@ -62,15 +62,15 @@
             >>> from wmflib.prometheus import Prometheus
             >>> prometheus = Prometheus()
 
     """
 
     _prometheus_api: str = 'http://prometheus.svc.{site}.wmnet/{instance}/api/v1/query'
 
-    def query(self, query: str, site: str, *, instance: str = 'ops', timeout: TypeTimeout = 10.0) -> List[Dict]:
+    def query(self, query: str, site: str, *, instance: str = 'ops', timeout: TimeoutType = 10.0) -> List[Dict]:
         """Perform a generic query.
 
         Examples:
             ::
 
                 >>> results = prometheus.query('node_uname_info{instance=~"host1001:.*"}', 'eqiad', instance='global')
                 >>> results = prometheus.query('node_memory_MemTotal_bytes{instance=~"host1001:.*"}', 'eqiad')
@@ -92,15 +92,15 @@
 
         Arguments:
             query (str): a prometheus query string.
             site (str): The site to use for queries. Must be one of
                 :py:const:`wmflib.constants.ALL_DATACENTERS`
             instance (str, optional): The prometheus instance to query on the given site, see
                 https://wikitech.wikimedia.org/wiki/Prometheus#Instances for the full list of available instances.
-            timeout (:py:data:`wmflib.requests.TypeTimeout`, optional): How many seconds to wait for prometheus to
+            timeout (:py:data:`wmflib.requests.TimeoutType`, optional): How many seconds to wait for prometheus to
                 reply before giving up. This is passed directly to the requests library.
 
         Returns:
             list: returns an empty list if there are no results otherwise return a list of results of the form:
             ``{'metric': {}, 'value': [$timestamp, $value]}``.
 
         Raises:
@@ -125,15 +125,15 @@
             >>> from wmflib.prometheus import Thanos
             >>> thanos = Thanos()
 
     """
 
     _thanos_api: str = 'https://thanos-query.discovery.wmnet/api/v1/query'
 
-    def query(self, query: str, *, timeout: TypeTimeout = 10.0) -> List[Dict]:
+    def query(self, query: str, *, timeout: TimeoutType = 10.0) -> List[Dict]:
         """Perform a generic query.
 
         Examples:
             ::
 
                 >>> results = thanos.query('node_memory_MemTotal_bytes{instance=~"host1001:.*"}')
                 >>> results = thanos.query('node_uname_info{instance=~"host1001:.*"}')
@@ -158,15 +158,15 @@
                         },
                         'value': [1648898872.82, '1']
                     }
                 ]
 
         Arguments:
             query (str): a prometheus query string.
-            timeout (:py:data:`wmflib.requests.TypeTimeout`, optional): How many seconds to wait for prometheus to
+            timeout (:py:data:`wmflib.requests.TimeoutType`, optional): How many seconds to wait for prometheus to
                 reply before giving up. This is passed directly to the requests library.
 
         Returns:
             list: returns an empty list if there are no results otherwise return a list of results of the form:
             ``{'metric': {}, 'value': [$timestamp, $value]}``.
 
         Raises:
```

### Comparing `wmflib-1.2.1/wmflib/requests.py` & `wmflib-1.2.2/wmflib/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from requests import PreparedRequest, Response, Session
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry  # pylint: disable=import-error
 
 from wmflib import __version__
 
 
-TypeTimeout = Union[float, Tuple[float, float]]
+TimeoutType = Union[float, Tuple[float, float]]
 """Type alias for the requests timeout parameter."""
-DEFAULT_TIMEOUT: TypeTimeout = (3.0, 5.0)
+DEFAULT_TIMEOUT: TimeoutType = (3.0, 5.0)
 """:py:class:`tuple`: the default timeout to use if none is passed, in seconds."""
 DEFAULT_RETRY_STATUS_CODES: Tuple[int, ...] = (429, 500, 502, 503, 504)
 """:py:class`tuple`: the default sequence of HTTP status codes that are retried if the method is one of
    :py:const:`DEFAULT_RETRY_METHODS`."""
 DEFAULT_RETRY_METHODS: Tuple[str, ...] = ('DELETE', 'GET', 'HEAD', 'OPTIONS', 'PUT', 'TRACE')
 """:py:class`tuple`: the default sequence of HTTP methods that are retried if the status code is one of
    :py:const:`DEFAULT_RETRY_STATUS_CODES`."""
@@ -58,15 +58,15 @@
         """
         if kwargs.get('timeout') is None:  # The Session will pass timeout=None when not set by the caller.
             kwargs['timeout'] = self.timeout
 
         return super().send(request, **kwargs)
 
 
-def http_session(name: str, *, timeout: TypeTimeout = DEFAULT_TIMEOUT, tries: int = 3, backoff: float = 1.0,
+def http_session(name: str, *, timeout: TimeoutType = DEFAULT_TIMEOUT, tries: int = 3, backoff: float = 1.0,
                  retry_codes: Sequence[int] = DEFAULT_RETRY_STATUS_CODES,
                  retry_methods: Sequence[str] = DEFAULT_RETRY_METHODS) -> Session:
     """Return a new requests Session with User-Agent, default timeout and retry logic on failure already setup.
 
     By default the returned session will retry any :py:const:`DEFAULT_RETRY_METHODS` request that returns one of
     the following HTTP status code (see :py:const:`DEFAULT_RETRY_STATUS_CODES`):
 
@@ -104,15 +104,15 @@
         https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
 
     Arguments:
         name (str): the name to use for the User-Agent header. It can be specified in the ``name/version`` format, if
             applicable. The resulting header will be set to::
 
                 pywmflib/{version} {name} +https://wikitech.wikimedia.org/wiki/Python/Wmflib root@wikimedia.org
-        timeout (:py:data:`wmflib.requests.TypeTimeout`): the default timeout to use in all requests within this
+        timeout (:py:data:`wmflib.requests.TimeoutType`): the default timeout to use in all requests within this
             session, in seconds. Any request can override it passing the ``timeout`` parameter explicitely. It can be
             either a single float or a tuple of two floats (connect, read), according to requests's documentation.
         tries (int): the total number of requests to perform before bailing out. If set to ``0`` the whole retry logic
             is not added to the session, making all the other parameters except the ``name`` one to be ignored. In this
             case only the User-Agent and default timeout are set.
         backoff (float): the backoff factor to use, will generate a sleep between retries, in seconds, of::
```

### Comparing `wmflib-1.2.1/wmflib/tests/__init__.py` & `wmflib-1.2.2/wmflib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/sphinx_checker.py` & `wmflib-1.2.2/wmflib/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_actions.py` & `wmflib-1.2.2/wmflib/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_config.py` & `wmflib-1.2.2/wmflib/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_decorators.py` & `wmflib-1.2.2/wmflib/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_dns.py` & `wmflib-1.2.2/wmflib/tests/unit/test_dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,8 +172,8 @@
 
 
 @mock.patch('wmflib.dns.resolver.Resolver')
 def test_public_auth_dns_init(mocked_resolver):
     """The Production nameservers should be set on the resolver."""
     PublicAuthDns()
     mocked_resolver.assert_called_once_with(configure=False)
-    assert mocked_resolver.return_value.nameservers == PUBLIC_AUTHDNS
+    assert mocked_resolver.return_value.nameservers == list(PUBLIC_AUTHDNS)
```

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_fileio.py` & `wmflib-1.2.2/wmflib/tests/unit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_idm.py` & `wmflib-1.2.2/wmflib/tests/unit/test_idm.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_interactive.py` & `wmflib-1.2.2/wmflib/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_irc.py` & `wmflib-1.2.2/wmflib/tests/unit/test_irc.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_phabricator.py` & `wmflib-1.2.2/wmflib/tests/unit/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_prometheus.py` & `wmflib-1.2.2/wmflib/tests/unit/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib/tests/unit/test_requests.py` & `wmflib-1.2.2/wmflib/tests/unit/test_requests.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.1/wmflib.egg-info/PKG-INFO` & `wmflib-1.2.2/wmflib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmflib
-Version: 1.2.1
+Version: 1.2.2
 Summary: Generic library for common tasks in the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-pywmflib
 Author: Luca Toscano
 Author-email: ltoscano@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation
 Platform: GNU/Linux
```

### Comparing `wmflib-1.2.1/wmflib.egg-info/SOURCES.txt` & `wmflib-1.2.2/wmflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

