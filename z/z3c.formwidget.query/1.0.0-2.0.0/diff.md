# Comparing `tmp/z3c.formwidget.query-1.0.0.tar.gz` & `tmp/z3c.formwidget.query-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.formwidget.query-1.0.0.tar", last modified: Wed Sep  7 20:36:54 2022, max compression
+gzip compressed data, was "z3c.formwidget.query-2.0.0.tar", last modified: Wed Apr 26 22:42:05 2023, max compression
```

## Comparing `z3c.formwidget.query-1.0.0.tar` & `z3c.formwidget.query-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.143549 z3c.formwidget.query-1.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)       32 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/AUTHOR.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1875 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      804 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)       32 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/COPYRIGHT.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2070 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      335 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     3664 2022-09-07 20:36:54.143647 z3c.formwidget.query-1.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      583 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      145 2022-09-07 20:36:54.144025 z3c.formwidget.query-1.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2010 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.133118 z3c.formwidget.query-1.0.0/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.137277 z3c.formwidget.query-1.0.0/src/z3c/
--rw-r--r--   0 maurits    (501) staff       (20)       76 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.139745 z3c.formwidget.query-1.0.0/src/z3c/formwidget/
--rw-r--r--   0 maurits    (501) staff       (20)       76 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.141640 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/
--rw-r--r--   0 maurits    (501) staff       (20)    11706 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)      102 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      213 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/configure.zcml
--rwxr-xr-x   0 maurits    (501) staff       (20)      700 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/i18n.sh
--rw-r--r--   0 maurits    (501) staff       (20)      225 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.142223 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.133656 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.142450 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      612 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/en/LC_MESSAGES/z3c.formwidget.query.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.133850 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.142669 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      626 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/it/LC_MESSAGES/z3c.formwidget.query.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.134044 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.143057 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      749 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/nl/LC_MESSAGES/z3c.formwidget.query.po
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/z3c.formwidget.query-manual.pot
--rw-r--r--   0 maurits    (501) staff       (20)      738 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/z3c.formwidget.query.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.134241 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/zh_CN/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.143367 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)      630 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/zh_CN/LC_MESSAGES/z3c.formwidget.query.po
--rw-r--r--   0 maurits    (501) staff       (20)      569 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)    10204 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-09-07 20:36:54.139384 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     3664 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1227 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       19 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      146 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        4 2022-09-07 20:36:54.000000 z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1190 2022-09-07 20:36:53.000000 z3c.formwidget.query-1.0.0/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.891223 z3c.formwidget.query-2.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)       32 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/AUTHOR.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2023 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      804 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 maurits    (501) staff       (20)       32 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/COPYRIGHT.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      335 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     3687 2023-04-26 22:42:05.891329 z3c.formwidget.query-2.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      583 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      423 2023-04-26 22:42:05.891783 z3c.formwidget.query-2.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1877 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.879778 z3c.formwidget.query-2.0.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.884866 z3c.formwidget.query-2.0.0/src/z3c/
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.887297 z3c.formwidget.query-2.0.0/src/z3c/formwidget/
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.889197 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/
+-rw-r--r--   0 maurits    (501) staff       (20)    11706 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      213 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/configure.zcml
+-rwxr-xr-x   0 maurits    (501) staff       (20)      700 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/i18n.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      225 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.889812 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.880850 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.890134 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      612 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/en/LC_MESSAGES/z3c.formwidget.query.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.881230 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.890414 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      626 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/it/LC_MESSAGES/z3c.formwidget.query.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.881482 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.890692 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/nl/LC_MESSAGES/z3c.formwidget.query.po
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/z3c.formwidget.query-manual.pot
+-rw-r--r--   0 maurits    (501) staff       (20)      738 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/z3c.formwidget.query.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.881729 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/zh_CN/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.891019 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      630 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/zh_CN/LC_MESSAGES/z3c.formwidget.query.po
+-rw-r--r--   0 maurits    (501) staff       (20)      602 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10203 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:42:05.887040 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     3687 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1227 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       19 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        4 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1389 2023-04-26 22:42:05.000000 z3c.formwidget.query-2.0.0/tox.ini
```

### Comparing `z3c.formwidget.query-1.0.0/CHANGES.rst` & `z3c.formwidget.query-2.0.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+2.0.0 (2023-04-27)
+------------------
+
+Breaking changes:
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+New features:
+
+- Add support for Python 3.11.
+
+
 1.0.0 (2022-09-07)
 ------------------
 
 - Add Chinese translation.
 
 - Add support for Python 3.5, 3.8, 3.9, 3.10.
```

### Comparing `z3c.formwidget.query-1.0.0/CONTRIBUTING.md` & `z3c.formwidget.query-2.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/LICENSE.txt` & `z3c.formwidget.query-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/PKG-INFO` & `z3c.formwidget.query-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: z3c.formwidget.query
-Version: 1.0.0
+Version: 2.0.0
 Summary: A source query widget for z3c.form.
 Home-page: https://github.com/zopefoundation/z3c.formwidget.query
 Author: Zope Community
-Author-email: zope3-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope zope3 z3c.form
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Zope :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Overview
 ========
 
 This package implements a widget that lets users enter a query and
@@ -48,14 +46,26 @@
 [1] The source needs to implement ``IQuerySource`` as defined in this
 package.
 
 
 Changelog
 =========
 
+2.0.0 (2023-04-27)
+------------------
+
+Breaking changes:
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+New features:
+
+- Add support for Python 3.11.
+
+
 1.0.0 (2022-09-07)
 ------------------
 
 - Add Chinese translation.
 
 - Add support for Python 3.5, 3.8, 3.9, 3.10.
```

### Comparing `z3c.formwidget.query-1.0.0/README.rst` & `z3c.formwidget.query-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/README.txt` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/i18n.sh` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/i18n.sh`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/en/LC_MESSAGES/z3c.formwidget.query.po` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/en/LC_MESSAGES/z3c.formwidget.query.po`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/it/LC_MESSAGES/z3c.formwidget.query.po` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/it/LC_MESSAGES/z3c.formwidget.query.po`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/nl/LC_MESSAGES/z3c.formwidget.query.po` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/nl/LC_MESSAGES/z3c.formwidget.query.po`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/z3c.formwidget.query.pot` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/z3c.formwidget.query.pot`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/locales/zh_CN/LC_MESSAGES/z3c.formwidget.query.po` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/locales/zh_CN/LC_MESSAGES/z3c.formwidget.query.po`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/tests.py` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import doctest
 import unittest
-from zope import interface, component, schema
-from zope.testing.cleanup import cleanUp
+
 from z3c.form import testing
+from zope import component
+from zope import interface
+from zope import schema
+from zope.testing.cleanup import cleanUp
 
 
 def setUp(test):
     testing.setUp(test)
     test.globs.update(dict(
         interface=interface,
         component=component,
```

### Comparing `z3c.formwidget.query-1.0.0/src/z3c/formwidget/query/widget.py` & `z3c.formwidget.query-2.0.0/src/z3c/formwidget/query/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from itertools import chain
 
+import z3c.form.browser.checkbox
+import z3c.form.browser.radio
+import z3c.form.button
+import z3c.form.field
+import z3c.form.form
+import z3c.form.interfaces
+import z3c.form.term
+import z3c.form.widget
 import zope.component
 import zope.interface
 import zope.schema
 import zope.schema.interfaces
-
-from zope.security import checkPermission
-
+from zope.schema.interfaces import IContextSourceBinder
+from zope.schema.interfaces import ISource
 from zope.schema.vocabulary import SimpleVocabulary
-from zope.schema.interfaces import ISource, IContextSourceBinder
-
-import z3c.form.interfaces
-import z3c.form.button
-import z3c.form.form
-import z3c.form.field
-import z3c.form.widget
-import z3c.form.term
-import z3c.form.browser.radio
-import z3c.form.browser.checkbox
+from zope.security import checkPermission
 
 from z3c.formwidget.query import MessageFactory as _
 
+
 HAS_AC = True
 try:
     from AccessControl.interfaces import IRoleManager
 except ImportError:
     HAS_AC = False
 
 
@@ -58,40 +57,40 @@
 
     fields = z3c.form.field.Fields(
         zope.schema.TextLine(
             __name__='query',
             required=False))
 
     def __init__(self, context, request, prefix=None):
-        super(QuerySubForm, self).__init__(context, request)
+        super().__init__(context, request)
 
         if prefix is not None:
             self.prefix = prefix
 
-    @z3c.form.button.buttonAndHandler(_(u"Search"))
+    @z3c.form.button.buttonAndHandler(_("Search"))
     def search(self, action):
         data, errors = self.widgets.extract()
         if not errors:
             z3c.form.form.applyChanges(self, self.context, data)
 
 
-class QueryContext(object):
+class QueryContext:
     query = None
 
 
 class QuerySourceRadioWidget(z3c.form.browser.radio.RadioWidget):
     """Query source widget that allows single selection."""
 
     _radio = True
     _queryform = None
     _resultsform = None
     _bound_source = None
     ignoreMissing = False
 
-    noValueLabel = _(u'(nothing)')
+    noValueLabel = _('(nothing)')
 
     @property
     def source(self):
         """We need to bind the field to the context so that vocabularies
         appear as sources"""
         return self.field.bind(self.context).source
 
@@ -224,15 +223,15 @@
                 return
 
             # perform the search
 
             query = data['query']
             if query is not None:
                 query_terms = set(source.search(query))
-                tokens = set([term.token for term in terms])
+                tokens = {term.token for term in terms}
                 for term in query_terms:
                     if term.token not in tokens:
                         terms.append(term)
 
         # set terms
         self.terms = QueryTerms(
             self.context,
```

### Comparing `z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/PKG-INFO` & `z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: z3c.formwidget.query
-Version: 1.0.0
+Version: 2.0.0
 Summary: A source query widget for z3c.form.
 Home-page: https://github.com/zopefoundation/z3c.formwidget.query
 Author: Zope Community
-Author-email: zope3-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope zope3 z3c.form
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Zope :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Overview
 ========
 
 This package implements a widget that lets users enter a query and
@@ -48,14 +46,26 @@
 [1] The source needs to implement ``IQuerySource`` as defined in this
 package.
 
 
 Changelog
 =========
 
+2.0.0 (2023-04-27)
+------------------
+
+Breaking changes:
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+New features:
+
+- Add support for Python 3.11.
+
+
 1.0.0 (2022-09-07)
 ------------------
 
 - Add Chinese translation.
 
 - Add support for Python 3.5, 3.8, 3.9, 3.10.
```

### Comparing `z3c.formwidget.query-1.0.0/src/z3c.formwidget.query.egg-info/SOURCES.txt` & `z3c.formwidget.query-2.0.0/src/z3c.formwidget.query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.formwidget.query-1.0.0/tox.ini` & `z3c.formwidget.query-2.0.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
+    py311
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=77
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=77
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = z3c.formwidget.query
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

