# Comparing `tmp/plone.resource-2.1.4.tar.gz` & `tmp/plone.resource-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.resource-2.1.4.tar", last modified: Tue Jun 15 01:32:32 2021, max compression
+gzip compressed data, was "plone.resource-3.0.0.tar", last modified: Wed Apr 26 22:02:37 2023, max compression
```

## Comparing `plone.resource-2.1.4.tar` & `plone.resource-3.0.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.878290 plone.resource-2.1.4/
--rw-r--r--   0 ems174     (502) staff       (20)     4298 2021-06-15 01:32:32.000000 plone.resource-2.1.4/CHANGES.rst
--rw-r--r--   0 ems174     (502) staff       (20)       70 2021-06-15 01:32:32.000000 plone.resource-2.1.4/CONTRIBUTING.rst
--rw-r--r--   0 ems174     (502) staff       (20)      149 2021-06-15 01:32:32.000000 plone.resource-2.1.4/MANIFEST.in
--rw-r--r--   0 ems174     (502) staff       (20)    13094 2021-06-15 01:32:32.878383 plone.resource-2.1.4/PKG-INFO
--rw-r--r--   0 ems174     (502) staff       (20)     4900 2021-06-15 01:32:32.000000 plone.resource-2.1.4/README.rst
--rw-r--r--   0 ems174     (502) staff       (20)      279 2021-06-15 01:32:32.000000 plone.resource-2.1.4/TODO.rst
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.872030 plone.resource-2.1.4/docs/
--rw-r--r--   0 ems174     (502) staff       (20)    17987 2021-06-15 01:32:32.000000 plone.resource-2.1.4/docs/LICENSE.GPL
--rw-r--r--   0 ems174     (502) staff       (20)      729 2021-06-15 01:32:32.000000 plone.resource-2.1.4/docs/LICENSE.txt
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.872151 plone.resource-2.1.4/plone/
--rw-r--r--   0 ems174     (502) staff       (20)       80 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/__init__.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.875237 plone.resource-2.1.4/plone/resource/
--rw-r--r--   0 ems174     (502) staff       (20)       24 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/__init__.py
--rw-r--r--   0 ems174     (502) staff       (20)      580 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/browser.zcml
--rw-r--r--   0 ems174     (502) staff       (20)      616 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/caching.py
--rw-r--r--   0 ems174     (502) staff       (20)      439 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/caching.zcml
--rw-r--r--   0 ems174     (502) staff       (20)      298 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/configure.zcml
--rw-r--r--   0 ems174     (502) staff       (20)     9423 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/directory.py
--rw-r--r--   0 ems174     (502) staff       (20)      814 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/download.py
--rw-r--r--   0 ems174     (502) staff       (20)      477 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/events.py
--rw-r--r--   0 ems174     (502) staff       (20)     2710 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/file.py
--rw-r--r--   0 ems174     (502) staff       (20)      188 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/file.zcml
--rw-r--r--   0 ems174     (502) staff       (20)     3194 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/interfaces.py
--rw-r--r--   0 ems174     (502) staff       (20)     9318 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/manifest.py
--rw-r--r--   0 ems174     (502) staff       (20)      328 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/meta.zcml
--rw-r--r--   0 ems174     (502) staff       (20)      200 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/permissions.zcml
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.870546 plone.resource-2.1.4/plone/resource/profiles/
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.875818 plone.resource-2.1.4/plone/resource/profiles/default/
--rw-r--r--   0 ems174     (502) staff       (20)      318 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/profiles/default/componentregistry.xml
--rw-r--r--   0 ems174     (502) staff       (20)       70 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/profiles/default/metadata.xml
--rw-r--r--   0 ems174     (502) staff       (20)      191 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/profiles/default/rolemap.xml
--rw-r--r--   0 ems174     (502) staff       (20)      173 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/profiles/default/toolset.xml
--rw-r--r--   0 ems174     (502) staff       (20)      466 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/profiles.zcml
--rw-r--r--   0 ems174     (502) staff       (20)     1869 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/testing.py
--rw-r--r--   0 ems174     (502) staff       (20)      377 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/testing.zcml
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.877201 plone.resource-2.1.4/plone/resource/tests/
--rw-r--r--   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/__init__.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.870731 plone.resource-2.1.4/plone/resource/tests/resources/
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.870846 plone.resource-2.1.4/plone/resource/tests/resources/demo/
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.877352 plone.resource-2.1.4/plone/resource/tests/resources/demo/foo/
--rw-r--r--   0 ems174     (502) staff       (20)        4 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/resources/demo/foo/test.html
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.877645 plone.resource-2.1.4/plone/resource/tests/resources/demo/manifest-test/
--rw-r--r--   0 ems174     (502) staff       (20)       85 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/resources/demo/manifest-test/manifest.cfg
--rw-r--r--   0 ems174     (502) staff       (20)        9 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/resources/demo/manifest-test/test.txt
--rw-r--r--   0 ems174     (502) staff       (20)      912 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/resources.zip
--rw-r--r--   0 ems174     (502) staff       (20)    10488 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_directory.py
--rw-r--r--   0 ems174     (502) staff       (20)     2278 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_file.py
--rw-r--r--   0 ems174     (502) staff       (20)     1001 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_integration.py
--rw-r--r--   0 ems174     (502) staff       (20)     9252 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_manifest.py
--rw-r--r--   0 ems174     (502) staff       (20)     4247 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_traversal.py
--rw-r--r--   0 ems174     (502) staff       (20)     4061 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_utils.py
--rw-r--r--   0 ems174     (502) staff       (20)     3183 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_zcml.py
--rw-r--r--   0 ems174     (502) staff       (20)     2919 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/test_zip_download.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.878194 plone.resource-2.1.4/plone/resource/tests/zipfiles/
--rw-r--r--   0 ems174     (502) staff       (20)      524 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/zipfiles/manifest-name-override.zip
--rw-r--r--   0 ems174     (502) staff       (20)     1002 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip
--rw-r--r--   0 ems174     (502) staff       (20)      316 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/zipfiles/no-manifest.zip
--rw-r--r--   0 ems174     (502) staff       (20)      348 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/zipfiles/no-top-level-dir.zip
--rw-r--r--   0 ems174     (502) staff       (20)      512 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/tests/zipfiles/normal.zip
--rw-r--r--   0 ems174     (502) staff       (20)     1058 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/traversal.py
--rw-r--r--   0 ems174     (502) staff       (20)     3410 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/utils.py
--rw-r--r--   0 ems174     (502) staff       (20)     2740 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone/resource/zcml.py
-drwxr-xr-x   0 ems174     (502) staff       (20)        0 2021-06-15 01:32:32.872971 plone.resource-2.1.4/plone.resource.egg-info/
--rw-r--r--   0 ems174     (502) staff       (20)    13094 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/PKG-INFO
--rw-r--r--   0 ems174     (502) staff       (20)     1980 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/SOURCES.txt
--rw-r--r--   0 ems174     (502) staff       (20)        1 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/dependency_links.txt
--rw-r--r--   0 ems174     (502) staff       (20)       53 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/entry_points.txt
--rw-r--r--   0 ems174     (502) staff       (20)        6 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/namespace_packages.txt
--rw-r--r--   0 ems174     (502) staff       (20)        1 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/not-zip-safe
--rw-r--r--   0 ems174     (502) staff       (20)      205 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/requires.txt
--rw-r--r--   0 ems174     (502) staff       (20)        6 2021-06-15 01:32:32.000000 plone.resource-2.1.4/plone.resource.egg-info/top_level.txt
--rw-r--r--   0 ems174     (502) staff       (20)      397 2021-06-15 01:32:32.000000 plone.resource-2.1.4/pyproject.toml
--rw-r--r--   0 ems174     (502) staff       (20)       67 2021-06-15 01:32:32.878587 plone.resource-2.1.4/setup.cfg
--rw-r--r--   0 ems174     (502) staff       (20)     1695 2021-06-15 01:32:32.000000 plone.resource-2.1.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.203117 plone.resource-3.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     4486 2023-04-26 22:02:36.000000 plone.resource-3.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 22:02:36.000000 plone.resource-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 22:02:36.000000 plone.resource-3.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    10239 2023-04-26 22:02:37.203238 plone.resource-3.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4900 2023-04-26 22:02:36.000000 plone.resource-3.0.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      279 2023-04-26 22:02:36.000000 plone.resource-3.0.0/TODO.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.187897 plone.resource-3.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-26 22:02:36.000000 plone.resource-3.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      729 2023-04-26 22:02:36.000000 plone.resource-3.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.188269 plone.resource-3.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.196836 plone.resource-3.0.0/plone/resource/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      596 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/browser.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/caching.py
+-rw-r--r--   0 maurits    (501) staff       (20)      446 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/caching.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9151 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/directory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/download.py
+-rw-r--r--   0 maurits    (501) staff       (20)      477 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2597 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      189 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/file.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3133 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8659 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/manifest.py
+-rw-r--r--   0 maurits    (501) staff       (20)      321 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.184425 plone.resource-3.0.0/plone/resource/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.198004 plone.resource-3.0.0/plone/resource/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      308 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/profiles/default/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/profiles/default/rolemap.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      178 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/profiles/default/toolset.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      472 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.200710 plone.resource-3.0.0/plone/resource/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.184811 plone.resource-3.0.0/plone/resource/tests/resources/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.185052 plone.resource-3.0.0/plone/resource/tests/resources/demo/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.200960 plone.resource-3.0.0/plone/resource/tests/resources/demo/foo/
+-rw-r--r--   0 maurits    (501) staff       (20)        4 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/resources/demo/foo/test.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.201525 plone.resource-3.0.0/plone/resource/tests/resources/demo/manifest-test/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/resources/demo/manifest-test/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/resources/demo/manifest-test/test.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      912 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/resources.zip
+-rw-r--r--   0 maurits    (501) staff       (20)    10453 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_directory.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2189 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_integration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9542 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_manifest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4158 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4096 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3306 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_zcml.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2892 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/test_zip_download.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.202911 plone.resource-3.0.0/plone/resource/tests/zipfiles/
+-rw-r--r--   0 maurits    (501) staff       (20)      524 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/zipfiles/manifest-name-override.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      316 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/zipfiles/no-manifest.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      348 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/zipfiles/no-top-level-dir.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      512 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/tests/zipfiles/normal.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3442 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2693 2023-04-26 22:02:36.000000 plone.resource-3.0.0/plone/resource/zcml.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:02:37.190436 plone.resource-3.0.0/plone.resource.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    10239 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1980 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:02:37.000000 plone.resource-3.0.0/plone.resource.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2858 2023-04-26 22:02:36.000000 plone.resource-3.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 22:02:37.203747 plone.resource-3.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1612 2023-04-26 22:02:36.000000 plone.resource-3.0.0/setup.py
```

### Comparing `plone.resource-2.1.4/CHANGES.rst` & `plone.resource-3.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-27)
+------------------
+
+Breaking changes:
+
+
+- Drop Plone 5.2 and Python 2 support.
+  [gforcada] (#6)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (2a4ba395)
+
+
 2.1.4 (2021-06-14)
 ------------------
 
 Bug fixes:
 
 
 - Do not throw an error when traversing to a FilesystemResourceDirectory (#31)
@@ -110,20 +127,20 @@
 
 
 1.1 (2016-10-04)
 ----------------
 
 New features:
 
-- Use ``mimetypes_registry`` utility to dertermine mimetype if available.
+- Use ``mimetypes_registry`` utility to determine mimetype if available.
   [jensens]
 
 Bug fixes:
 
-- Remove duplicte import
+- Remove duplicate import
   [jensens]
 
 - Add coding headers on python files.
   [gforcada]
 
 1.0.7 (2016-09-08)
 ------------------
```

### Comparing `plone.resource-2.1.4/README.rst` & `plone.resource-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/docs/LICENSE.GPL` & `plone.resource-3.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/docs/LICENSE.txt` & `plone.resource-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/plone/resource/browser.zcml` & `plone.resource-3.0.0/plone/resource/browser.zcml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
   <browser:view
       name="download-zip"
       for=".interfaces.IResourceDirectory"
-      permission="plone.resource.ExportZip"
       class=".download.DownloadView"
+      permission="plone.resource.ExportZip"
       />
 
   <!-- Unique traverser -->
   <adapter
-      name="unique"
-      for=".interfaces.IResourceDirectory zope.publisher.interfaces.IRequest"
-      provides="zope.traversing.interfaces.ITraversable"
       factory=".traversal.UniqueResourceTraverser"
+      provides="zope.traversing.interfaces.ITraversable"
+      for=".interfaces.IResourceDirectory
+           zope.publisher.interfaces.IRequest"
+      name="unique"
       />
 
 </configure>
```

### Comparing `plone.resource-2.1.4/plone/resource/caching.py` & `plone.resource-3.0.0/plone/resource/caching.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
 from plone.caching.interfaces import IRulesetLookup
 from plone.resource.interfaces import IUniqueResourceRequest
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 @implementer(IRulesetLookup)
 @adapter(Interface, IUniqueResourceRequest)
-class UniqueResourceLookup(object):
+class UniqueResourceLookup:
     """Unique resource ruleset lookup.
 
     Returns 'plone.stableResource' for requests marked with
     IUniqueResourceRequest.
     """
 
     def __init__(self, published, request):
         pass
 
     def __call__(self):
-        return 'plone.stableResource'
+        return "plone.stableResource"
```

### Comparing `plone.resource-2.1.4/plone/resource/directory.py` & `plone.resource-3.0.0/plone/resource/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from Acquisition import aq_parent
 from OFS.Image import File
 from OFS.interfaces import IObjectManager
 from plone.resource.events import PloneResourceCreatedEvent
 from plone.resource.events import PloneResourceModifiedEvent
 from plone.resource.file import FilesystemFile
@@ -12,163 +11,156 @@
 from Products.CMFCore.utils import getToolByName
 from zExceptions import Forbidden
 from zExceptions import NotFound
 from zope.component.hooks import getSite
 from zope.event import notify
 from zope.interface import implementer
 
+import io
 import os.path
 import re
-import six
 import zipfile
 
 
 # filter dot files, Mac resource forks
-FILTERS = (r'\..*', '__MACOSX')
+FILTERS = (r"\..*", "__MACOSX")
 FILTERS = [re.compile(pattern) for pattern in FILTERS]
 
 
 @implementer(IWritableResourceDirectory)
-class PersistentResourceDirectory(object):
+class PersistentResourceDirectory:
     """A resource directory stored in the ZODB.
 
     It is assumed that directories provide IObjectManager
     and that files are instances of OFS.Image.File.
     """
 
     def __init__(self, context=None):
         if context is None:
             # This is also used as a local IResourceDirectory utility,
             # named u'persistent', which wraps the root folder.
             # This gets pickled, so we can't keep the acquisition chain.
-            context = aq_base(getToolByName(getSite(), 'portal_resources'))
+            context = aq_base(getToolByName(getSite(), "portal_resources"))
         self.context = self.__parent__ = context
         self.__name__ = context.getId()
 
     def __repr__(self):
-        return '<%s object at %s>' % (self.__class__.__name__,
-                                      '/'.join(self.context.getPhysicalPath()))
+        return "<{} object at {}>".format(
+            self.__class__.__name__, "/".join(self.context.getPhysicalPath())
+        )
 
     def publishTraverse(self, request, name):
-        if six.PY2 and isinstance(name, six.text_type):
-            name = name.encode('utf-8')
-
         context = self.context
         if aq_parent(context) is None:
             # Re-supply the acquisition chain if this is the root resource
             # directory, so that security checks work.
             site = getSite()
             if site is not None:
                 context = context.__of__(site)
 
         if self.isDirectory(name):
-            return self.__class__(
-                context.unrestrictedTraverse(name).__of__(context)
-            )
+            return self.__class__(context.unrestrictedTraverse(name).__of__(context))
         elif self.isFile(name):
             return context.unrestrictedTraverse(name).__of__(context)
 
         raise NotFound
 
     def __getitem__(self, name):
         return self.publishTraverse(None, name)
 
     def __setitem__(self, name, item):
-        if six.PY2 and isinstance(name, six.text_type):
-            name = name.encode('utf-8')
-
         if IResourceDirectory.providedBy(item):
             item = item.context
         self.context[name] = item
         item.id = item.__name__ = name
 
     def __delitem__(self, name):
         del self.context[name]
 
     def __contains__(self, name):
         return name in self.context
 
     def openFile(self, path):
-        return six.BytesIO(self.readFile(path))
+        return io.BytesIO(self.readFile(path))
 
     def readFile(self, path):
         try:
             f = self.context.unrestrictedTraverse(path)
         except Exception as e:
-            raise IOError(str(e))
-        if isinstance(f.data, six.binary_type):
+            raise OSError(str(e))
+        if isinstance(f.data, bytes):
             return f.data
         return f.data.__bytes__()
 
     def listDirectory(self):
-        return [n for n in self.context.objectIds()
-                if not any(filter.match(n) for filter in FILTERS)]
+        return [
+            n
+            for n in self.context.objectIds()
+            if not any(filter.match(n) for filter in FILTERS)
+        ]
 
     def isDirectory(self, path):
         try:
             obj = self.context.unrestrictedTraverse(path)
-        except:
+        except Exception:
             obj = None
 
         return IObjectManager.providedBy(obj)
 
     def isFile(self, path):
         try:
             obj = self.context.unrestrictedTraverse(path)
-        except:
+        except Exception:
             obj = None
 
         return isinstance(obj, File)
 
     def rename(self, oldName, newName):
         obj = self.context[oldName]
         obj.id = obj.__name__ = newName
         self.context._delOb(oldName)
         self.context._setOb(newName, obj)
 
     def exportZip(self, out):
         prefix = self.__name__
 
-        zf = zipfile.ZipFile(out, 'w')
+        zf = zipfile.ZipFile(out, "w")
 
         def write(dir, prefix, zf):
             for name in dir.listDirectory():
-                relativeName = "%s/%s" % (prefix, name,)
+                relativeName = f"{prefix}/{name}"
                 if dir.isDirectory(name):
                     write(dir[name], relativeName, zf)
                 elif dir.isFile(name):
                     zf.writestr(relativeName, dir.readFile(name))
 
         write(self, prefix, zf)
         zf.close()
 
     def makeDirectory(self, path):
-        if six.PY2:
-            path = path.encode('utf-8')
-
         parent = self.context
-        names = path.strip('/').split('/')
+        names = path.strip("/").split("/")
         for name in names:
             if name not in parent:
                 f = BTreeFolder2(name)
                 parent._setOb(name, f)
             parent = parent[name]
 
     def writeFile(self, path, data):
-        if isinstance(data, six.text_type):
-            data = data.encode('utf8')
-        basepath = '/'.join(path.split('/')[:-1])
+        if isinstance(data, str):
+            data = data.encode("utf8")
+        basepath = "/".join(path.split("/")[:-1])
         if basepath:
             self.makeDirectory(basepath)
-        filename = path.split('/')[-1]
+        filename = path.split("/")[-1]
         f = File(filename, filename, data)
         ct = f.getContentType()
-        if ct.startswith('text/') or ct == 'application/javascript':
+        if ct.startswith("text/") or ct == "application/javascript":
             # otherwise HTTPResponse.setBody assumes latin1 and mangles things
-            f.content_type = ct + '; charset=utf-8'
+            f.content_type = ct + "; charset=utf-8"
         container = self.context.unrestrictedTraverse(basepath)
         if filename in container:
             container._delOb(filename)
             event = PloneResourceModifiedEvent
         else:
             event = PloneResourceCreatedEvent
         container._setOb(filename, f)
@@ -176,33 +168,30 @@
         notify(event(obj))
 
     def importZip(self, f):
         if not isinstance(f, zipfile.ZipFile):
             f = zipfile.ZipFile(f)
         for name in f.namelist():
             member = f.getinfo(name)
-            path = member.filename.lstrip('/')
+            path = member.filename.lstrip("/")
 
             # test each part of the path against the filters
-            if any(any(filter.match(n) for filter in FILTERS)
-                   for n in path.split('/')
-                   ):
+            if any(any(filter.match(n) for filter in FILTERS) for n in path.split("/")):
                 continue
 
-            if path.endswith('/'):
+            if path.endswith("/"):
                 self.makeDirectory(path)
             else:
                 data = f.open(member).read()
                 self.writeFile(path, data)
 
 
 @implementer(IResourceDirectory)
-class FilesystemResourceDirectory(object):
-    """A resource directory based on files in the filesystem.
-    """
+class FilesystemResourceDirectory:
+    """A resource directory based on files in the filesystem."""
 
     __allow_access_to_unprotected_subobjects__ = True
 
     def __init__(self, directory, name=None, parent=None):
         self.directory = directory
         self.__name__ = name
         if name is None:
@@ -216,26 +205,24 @@
         return self._parent
 
     @__parent__.setter
     def __parent__(self, value):
         self._parent = value
 
     def __repr__(self):
-        return '<%s object at %s>' % (self.__class__.__name__, self.__name__)
+        return f"<{self.__class__.__name__} object at {self.__name__}>"
 
     def __bytes__(self):
-        if six.PY2:
-            return repr(self)
         return repr(self).encode()
 
     def _resolveSubpath(self, path):
-        parts = path.split('/')
+        parts = path.split("/")
         filepath = os.path.abspath(os.path.join(self.directory, *parts))
         if not filepath.startswith(self.directory):
-            raise Forbidden('Invalid path resource')
+            raise Forbidden("Invalid path resource")
         return filepath
 
     def publishTraverse(self, request, name):
         filepath = self._resolveSubpath(name)
         if self.isDirectory(name):
             return self.__class__(filepath, parent=self)
         elif self.isFile(name):
@@ -249,43 +236,48 @@
         return False
 
     def __getitem__(self, name):
         return self.publishTraverse(None, name)
 
     def openFile(self, path):
         filepath = self._resolveSubpath(path)
-        return open(filepath, 'rb')
+        return open(filepath, "rb")
 
     def readFile(self, path):
         with self.openFile(path) as f:
             return f.read()
 
     def listDirectory(self):
         names = os.listdir(self.directory)
-        return [n for n in names
-                if not any(filter.match(n) for filter in FILTERS)]
+        return [n for n in names if not any(filter.match(n) for filter in FILTERS)]
 
     def isDirectory(self, path):
         return os.path.isdir(self._resolveSubpath(path))
 
     def isFile(self, path):
         return os.path.isfile(self._resolveSubpath(path))
 
     def exportZip(self, out):
-        with zipfile.ZipFile(out, 'w') as zf:
-            toStrip = len(self.directory.replace(os.path.sep, '/')) + 1
+        with zipfile.ZipFile(out, "w") as zf:
+            toStrip = len(self.directory.replace(os.path.sep, "/")) + 1
 
-            for (dirpath, dirnames, filenames) in os.walk(self.directory):
-                subpath = dirpath.replace(os.path.sep, '/')[toStrip:].strip('/')
+            for dirpath, dirnames, filenames in os.walk(self.directory):
+                subpath = dirpath.replace(os.path.sep, "/")[toStrip:].strip("/")
 
                 for filename in filenames:
-                    path = '/'.join([subpath, filename]).strip('/')
+                    path = "/".join([subpath, filename]).strip("/")
 
-                    if any(any(filter.match(n) for filter in FILTERS)
-                           for n in path.split('/')
-                           ):
+                    if any(
+                        any(filter.match(n) for filter in FILTERS)
+                        for n in path.split("/")
+                    ):
                         continue
 
                     zf.writestr(
-                        '/'.join([self.__name__, path, ]),
+                        "/".join(
+                            [
+                                self.__name__,
+                                path,
+                            ]
+                        ),
                         self.readFile(path),
                     )
```

### Comparing `plone.resource-2.1.4/plone/resource/file.py` & `plone.resource-3.0.0/plone/resource/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from datetime import time
 from dateutil.tz import tzlocal
 from email.utils import formatdate
 from z3c.caching.interfaces import ILastModified
 from zope.component import adapter
 from zope.component import queryUtility
 from zope.filerepresentation.interfaces import IRawReadFile
@@ -21,76 +20,69 @@
     This is needed for ResourceRegistries support, for example.
     """
 
     def __str__(self):
         return self.read()
 
     def __unicode__(self):
-        return self.read().decode('utf-8')
+        return self.read().decode("utf-8")
 
 
-class FilesystemFile(object):
+class FilesystemFile:
     """Representation of a file. When called, it will set response headers
     and return the file's contents
     """
 
     def __init__(self, parent, request, path, name):
         self.path = path
         self.request = request
         self.__name__ = name
         self.__parent__ = parent
-        self.lastModifiedTimestamp = float(
-            os.path.getmtime(path)
-        ) or time.time()
+        self.lastModifiedTimestamp = float(os.path.getmtime(path)) or time.time()
 
-    def getContentType(self, default='application/octet-stream'):
+    def getContentType(self, default="application/octet-stream"):
         extension = os.path.splitext(self.__name__)[1].lower()
-        mtr = queryUtility('mimetypes_registry')
+        mtr = queryUtility("mimetypes_registry")
         mt = None
         if mtr:
             mt = mtr.lookupExtension(extension)
         if mt is None:
             mt = mimetypes.types_map.get(extension, default)
         return mt
 
     def __call__(self, REQUEST=None, RESPONSE=None):
         contentType = self.getContentType()
-        lastModifiedHeader = formatdate(
-            self.lastModifiedTimestamp,
-            usegmt=True
-        )
+        lastModifiedHeader = formatdate(self.lastModifiedTimestamp, usegmt=True)
 
         request = REQUEST
         if request is None:
             request = self.request
 
         response = RESPONSE
         if response is None:
             response = self.request.response
 
-        response.setHeader('Content-Type', contentType)
-        response.setHeader('Content-Length', os.path.getsize(self.path))
-        response.setHeader('Last-Modified', lastModifiedHeader)
+        response.setHeader("Content-Type", contentType)
+        response.setHeader("Content-Length", os.path.getsize(self.path))
+        response.setHeader("Last-Modified", lastModifiedHeader)
 
-        return ResourceIterator(self.path, 'rb')
+        return ResourceIterator(self.path, "rb")
 
 
 @implementer(ILastModified)
 @adapter(FilesystemFile)
-class FileLastModified(object):
-    """Determine when a file was last modified, for caching purposes
-    """
+class FileLastModified:
+    """Determine when a file was last modified, for caching purposes"""
 
     def __init__(self, context):
         self.context = context
 
     def __call__(self):
         return datetime.datetime.fromtimestamp(
-            self.context.lastModifiedTimestamp,
-            tz=tzlocal()
+            self.context.lastModifiedTimestamp, tz=tzlocal()
         )
 
 
 @implementer(IRawReadFile)
 @adapter(FilesystemFile)
 def rawReadFile(context):
-    return open(context.path, 'rb')
+    return open(context.path, "rb")
```

### Comparing `plone.resource-2.1.4/plone/resource/interfaces.py` & `plone.resource-3.0.0/plone/resource/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Attribute
 from zope.interface import Interface
 from zope.lifecycleevent.interfaces import IObjectCreatedEvent
 from zope.lifecycleevent.interfaces import IObjectModifiedEvent
 from zope.publisher.interfaces import IPublishTraverse
 
 
@@ -16,16 +15,15 @@
 
     __name__ = Attribute("""The name of the directory.""")
 
     def __repr__():
         """Returns a string identifier of the directory."""
 
     def __contains__(name):
-        """Return true if the given file or directory exists
-        """
+        """Return true if the given file or directory exists"""
 
     def __getitem__(name):
         """Return the file or resource directory with the given name
         as an object
         """
 
     def openFile(path):
@@ -58,15 +56,14 @@
     def exportZip(out):
         """Exports the contents of this directory as a zip file, which will
         be written to the open file handle ``out``.
         """
 
 
 class IWritableResourceDirectory(IResourceDirectory):
-
     def makeDirectory(path):
         """Create the given path as a directory. (Returns successfully without
         doing anything if the directory already exists.)
         """
 
     def writeFile(path, data):
         """Write a file at the specified path.
@@ -81,24 +78,21 @@
         """Imports the contents of a zip file into this directory.
 
         ``file`` may be a filename, file-like object, or instance of
         zipfile.ZipFile. The file data must be a ZIP archive.
         """
 
     def __delitem__(name):
-        """Delete a file or directory inside this directory
-        """
+        """Delete a file or directory inside this directory"""
 
     def __setitem__(name, item):
-        """Add a file or directory as returned by ``__getitem__()``
-        """
+        """Add a file or directory as returned by ``__getitem__()``"""
 
     def rename(oldName, newName):
-        """Rename a child file or folder
-        """
+        """Rename a child file or folder"""
 
 
 class IUniqueResourceRequest(Interface):
     """Marker interface for requests to ++unique++<id>"""
 
 
 class IPloneResourceCreatedEvent(IObjectCreatedEvent):
```

### Comparing `plone.resource-2.1.4/plone/resource/manifest.py` & `plone.resource-3.0.0/plone/resource/manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Utilities for working with manifest files.
 
 The manifest is stored in a file ``manifest.cfg`` in the root of a resource
 directory. It uses ini file (ConfigParser) syntax.
 
 For example, for the resource type foo, there could be a manifest file like::
 
@@ -24,38 +23,29 @@
     from plone.resource.manifest import getManifest
     manifest = getManifest(fp, FOO_FORMAT)
 
 ``manifest`` will now be a dict with keys ``title``, ``description``, and
 ``bar``. ``title`` and ``description`` will be ``None`` if not found in the
 manifest. ``bar`` will be ``baz`` if not found.
 """
+from configparser import ConfigParser
 from plone.resource.directory import FILTERS
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.utils import iterDirectoriesOfType
 from zope.component import getUtility
 
 import logging
-import six
 
-try:
-    # On Python 2 we must have the SafeConfigParser
-    from ConfigParser import SafeConfigParser as ConfigParser
-except ImportError:
-    # On Python 3 we want the standard ConfigParser,
-    # to avoid a deprecation warning.
-    # Note that on Python 2 configparser can come from a backport.
-    from configparser import ConfigParser
 
+MANIFEST_FILENAME = "manifest.cfg"
 
-MANIFEST_FILENAME = 'manifest.cfg'
+LOGGER = logging.getLogger("plone.resource.manifest")
 
-LOGGER = logging.getLogger('plone.resource.manifest')
 
-
-class ManifestFormat(object):
+class ManifestFormat:
     """Describes a manifest format.
 
     An immutable, threadsafe object.
 
     ``resourceType`` is used as the section header.
 
     ``keys`` should be a list of keys that should be returned.
@@ -66,16 +56,15 @@
     ``parameterSections`` can be a list section names in the ``manifest.cfg``
     file that can be used to supply additional, free-form parameters. For
     example, if ``parameters`` is ['parameters'] and 'resourceType' is
     'theme', then the ``manifest.cfg`` file may optionally contain a section
     ``[theme:parameters]``.
     """
 
-    def __init__(self, resourceType, keys, defaults=None,
-                 parameterSections=None):
+    def __init__(self, resourceType, keys, defaults=None, parameterSections=None):
         self.resourceType = resourceType
         self.keys = keys
         self.defaults = defaults or {}
         self.parameterSections = parameterSections or []
 
 
 def getManifest(fp, format, defaults=None):
@@ -84,41 +73,39 @@
     from the manifest format.
     """
 
     if defaults is None:
         defaults = format.defaults
 
     parser = ConfigParser()
-    if six.PY2:
-        parser.readfp(fp)
-    else:
-        data = fp.read()
-        if isinstance(data, six.binary_type):
-            data = data.decode()
-        parser.read_string(data)
+    data = fp.read()
+    if isinstance(data, bytes):
+        data = data.decode()
+    parser.read_string(data)
 
     results = {}
     for key in format.keys:
         if parser.has_option(format.resourceType, key):
             results[key] = parser.get(format.resourceType, key)
         else:
             results[key] = defaults.get(key, None)
 
     for key in format.parameterSections:
-        sectionName = "%s:%s" % (format.resourceType, key,)
+        sectionName = f"{format.resourceType}:{key}"
         if parser.has_section(sectionName):
             results[key] = dict(parser.items(sectionName))
         else:
             results[key] = {}
 
     return results
 
 
-def extractManifestFromZipFile(zipfile, format, defaults=None,
-                               manifestFilename=MANIFEST_FILENAME):
+def extractManifestFromZipFile(
+    zipfile, format, defaults=None, manifestFilename=MANIFEST_FILENAME
+):
     """Get a resource name and manifest from the given open
     ``zipfile.ZipFile`` using the given format. Returns a tuple::
 
         (resourceName, manifestDict)
 
     Where ``resourceName`` is the resource name, taken to be the name of the
     single top level directory inside the zip file (ignoring certain OS
@@ -136,64 +123,59 @@
     """
 
     resourceName = None
     manifestDict = None
 
     for name in zipfile.namelist():
         member = zipfile.getinfo(name)
-        path = member.filename.lstrip('/')
+        path = member.filename.lstrip("/")
 
         # Skip filtered files (OS X junk and dot files, mainly)
-        if any(
-            any(
-                filter.match(n) for filter in FILTERS
-            ) for n in path.split('/')
-        ):
+        if any(any(filter.match(n) for filter in FILTERS) for n in path.split("/")):
             continue
 
-        pathSegments = path.rstrip('/').split('/')
-        isDirectory = path.endswith('/')
+        pathSegments = path.rstrip("/").split("/")
+        isDirectory = path.endswith("/")
 
         # Is this a new top level directory?
         if pathSegments[0] != resourceName:
-
             # We already thought we had one - abort
             if resourceName is not None:
                 raise ValueError("More than one top level directory")
 
             # Store the first path segment (which may either be the directory)
             # itself, or the directory part in which some file is found
             if isDirectory or len(pathSegments) > 0:
                 resourceName = pathSegments[0]
             else:
                 raise ValueError(
-                    "Found a top level file - expected a single top level "
-                    "directory"
+                    "Found a top level file - expected a single top level " "directory"
                 )
 
         # Did we find a manifest file?
         if (
-            resourceName is not None and
-            not isDirectory and
-            path == "%s/%s" % (resourceName, manifestFilename,)
+            resourceName is not None
+            and not isDirectory
+            and path == f"{resourceName}/{manifestFilename}"
         ):
             manifest = zipfile.open(member)
             try:
                 manifestDict = getManifest(manifest, format, defaults=defaults)
             finally:
                 manifest.close()
 
     if resourceName is None:
         raise ValueError("No top level directory found")
 
     return (resourceName, manifestDict)
 
 
-def getAllResources(format, defaults=None, filter=None,
-                    manifestFilename=MANIFEST_FILENAME):
+def getAllResources(
+    format, defaults=None, filter=None, manifestFilename=MANIFEST_FILENAME
+):
     """Get a dict of all resources of the resource type indicated by the
     manifest format. Returns a dict where the keys are the resource ids and
     the values are manifests. The value may be None if no manifest was found.
 
     Pass ``defaults`` to override the defaults from the manifest format.
 
     Pass ``filter``, a callable that takes a resource directory as its
@@ -204,40 +186,35 @@
     Pass ``manifestFilename`` to use a different manifest file name
     convention.
     """
 
     resources = {}
 
     for directory in iterDirectoriesOfType(format.resourceType):
-
         if filter is not None and not filter(directory):
             continue
 
         name = directory.__name__
         resources[name] = None
 
         if directory.isFile(manifestFilename):
-
             manifest = directory.openFile(manifestFilename)
             try:
                 resources[name] = getManifest(manifest, format, defaults)
-            except:
-                LOGGER.exception(
-                    "Unable to read manifest for theme directory {0}".format(
-                        name
-                    )
-                )
+            except Exception:
+                LOGGER.exception(f"Unable to read manifest for theme directory {name}")
             finally:
                 manifest.close()
 
     return resources
 
 
-def getZODBResources(format, defaults=None, filter=None,
-                     manifestFilename=MANIFEST_FILENAME):
+def getZODBResources(
+    format, defaults=None, filter=None, manifestFilename=MANIFEST_FILENAME
+):
     """Get a dict of all resources in the ZODB of the resource type indicated
     by the manifest format. Returns a dict where the keys are the resource
     ids and the values are manifests. The value may be None if no manifest was
     found.
 
     Pass ``defaults`` to override the defaults from the manifest format.
 
@@ -255,29 +232,28 @@
     persistentDirectory = getUtility(IResourceDirectory, name="persistent")
     if format.resourceType not in persistentDirectory:
         return resources
 
     resourcesDirectory = persistentDirectory[format.resourceType]
 
     for name in resourcesDirectory.listDirectory():
-
         resourceDir = resourcesDirectory[name]
 
         if filter is not None and not filter(resourceDir):
             continue
 
         resources[name] = None
 
         if resourceDir.isFile(manifestFilename):
             manifest = resourceDir.openFile(MANIFEST_FILENAME)
             try:
                 resources[name] = getManifest(manifest, format, defaults)
-            except:
+            except Exception:
                 LOGGER.exception(
-                    "Unable to read manifest for {0} directory {1}".format(
+                    "Unable to read manifest for {} directory {}".format(
                         manifest.resourceType, name
                     )
                 )
             finally:
                 manifest.close()
 
     return resources
```

### Comparing `plone.resource-2.1.4/plone/resource/testing.py` & `plone.resource-3.0.0/plone/resource/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import applyProfile
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.resource.traversal import ResourceTraverser
 from plone.testing import Layer
 from plone.testing import publisher
@@ -13,52 +12,48 @@
 
 
 class DemoTraverser(Layer):
     defaultBases = (STARTUP, publisher.PUBLISHER_DIRECTIVES)
 
     def setUp(self):
         # Stack a new configuration context
-        self['configurationContext'] = context = zca.stackConfigurationContext(
-            self.get('configurationContext')
+        self["configurationContext"] = context = zca.stackConfigurationContext(
+            self.get("configurationContext")
         )
 
         import plone.resource
-        xmlconfig.file('testing.zcml', plone.resource, context=context)
+
+        xmlconfig.file("testing.zcml", plone.resource, context=context)
 
     def tearDown(self):
         # Zap the stacked configuration context
-        del self['configurationContext']
+        del self["configurationContext"]
 
 
 DEMO_TRAVERSER_FIXTURE = DemoTraverser()
 DEMO_TRAVERSER_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(DEMO_TRAVERSER_FIXTURE,),
-    name="plone.resource:DemoTraverserFunctional"
+    bases=(DEMO_TRAVERSER_FIXTURE,), name="plone.resource:DemoTraverserFunctional"
 )
 
 
 class PloneResource(PloneSandboxLayer):
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load ZCML
         import plone.resource
-        xmlconfig.file(
-            'configure.zcml',
-            plone.resource,
-            context=configurationContext
-        )
+
+        xmlconfig.file("configure.zcml", plone.resource, context=configurationContext)
 
     def setUpPloneSite(self, portal):
         # install into the Plone site
-        applyProfile(portal, 'plone.resource:default')
+        applyProfile(portal, "plone.resource:default")
 
 
 PLONE_RESOURCE_FIXTURE = PloneResource()
 PLONE_RESOURCE_INTEGRATION_TESTING = IntegrationTesting(
-    bases=(PLONE_RESOURCE_FIXTURE,),
-    name="plone.resource:Integration"
+    bases=(PLONE_RESOURCE_FIXTURE,), name="plone.resource:Integration"
 )
 
 
 class DemoTraverser(ResourceTraverser):
-    name = 'demo'
+    name = "demo"
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/resources.zip` & `plone.resource-3.0.0/plone/resource/tests/resources.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_directory.py` & `plone.resource-3.0.0/plone/resource/tests/test_directory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,302 +1,304 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from io import BytesIO
 from OFS.Image import File
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.directory import PersistentResourceDirectory
 from plone.resource.events import PloneResourceCreatedEvent
 from plone.resource.events import PloneResourceModifiedEvent
 from plone.resource.interfaces import IPloneResourceCreatedEvent
 from plone.resource.interfaces import IPloneResourceModifiedEvent
 from Products.BTreeFolder2.BTreeFolder2 import BTreeFolder2
 from zExceptions import NotFound
-from zipfile import ZipFile
 from zope.component import adapter
 from zope.component import provideHandler
 from zope.site.testing import createSiteManager
 from zope.site.testing import siteSetUp
 from zope.site.testing import siteTearDown
 
 import os.path
 import unittest
 
 
 class TestPersistentResourceDirectory(unittest.TestCase):
-
     def _makeOne(self):
-        root = BTreeFolder2('portal_resources')
-        root._setOb('demo', BTreeFolder2('demo'))
-        root.demo._setOb('foo', BTreeFolder2('foo'))
-        file = File('test.html', 'test.html', BytesIO(b'asdf'))
-        root.demo.foo._setOb('test.html', file)
+        root = BTreeFolder2("portal_resources")
+        root._setOb("demo", BTreeFolder2("demo"))
+        root.demo._setOb("foo", BTreeFolder2("foo"))
+        file = File("test.html", "test.html", BytesIO(b"asdf"))
+        root.demo.foo._setOb("test.html", file)
 
         return PersistentResourceDirectory(root)
 
     def _assertSameUnwrapped(self, a, b):
         self.assertTrue(aq_base(a) is aq_base(b))
 
     def test_ctor_implicit_context(self):
         siteSetUp()
 
-        site = BTreeFolder2('site')
+        site = BTreeFolder2("site")
         createSiteManager(site, setsite=True)
         root = self._makeOne().context
-        site._setOb('portal_resources', root)
+        site._setOb("portal_resources", root)
 
         try:
             dir = PersistentResourceDirectory()
             # context should be stored unwrapped
             self.assertTrue(aq_base(root) is dir.context)
 
             # but re-wrapped during traversal
-            traversed = dir['demo']
+            traversed = dir["demo"]
             self.assertTrue(site in traversed.context.aq_chain)
         finally:
             siteTearDown()
 
     def test_repr(self):
         dir = self._makeOne()
-        s = '<PersistentResourceDirectory object at portal_resources>'
+        s = "<PersistentResourceDirectory object at portal_resources>"
         self.assertEqual(s, repr(dir))
 
     def test_publishTraverse_directory(self):
         dir = self._makeOne()
-        subdir = dir.publishTraverse(None, 'demo')
+        subdir = dir.publishTraverse(None, "demo")
         self._assertSameUnwrapped(subdir.context, dir.context.demo)
 
     def test_publishTraverse_file(self):
         dir = self._makeOne()
-        file = dir.publishTraverse(None, 'demo/foo/test.html')
-        self._assertSameUnwrapped(file, dir.context.demo.foo['test.html'])
+        file = dir.publishTraverse(None, "demo/foo/test.html")
+        self._assertSameUnwrapped(file, dir.context.demo.foo["test.html"])
 
     def test_publishTraverse_not_found(self):
         dir = self._makeOne()
-        self.assertRaises(NotFound, dir.publishTraverse, None, 'baz')
+        self.assertRaises(NotFound, dir.publishTraverse, None, "baz")
 
     def test_getitem(self):
         dir = self._makeOne()
-        self._assertSameUnwrapped(dir['demo'].context, dir.context.demo)
+        self._assertSameUnwrapped(dir["demo"].context, dir.context.demo)
 
     def test_openFile(self):
         dir = self._makeOne()
-        file = dir.openFile('demo/foo/test.html')
-        self.assertEqual(b'asdf', file.read())
+        file = dir.openFile("demo/foo/test.html")
+        self.assertEqual(b"asdf", file.read())
 
     def test_readFile(self):
         dir = self._makeOne()
-        self.assertEqual(b'asdf', dir.readFile('demo/foo/test.html'))
+        self.assertEqual(b"asdf", dir.readFile("demo/foo/test.html"))
 
     def test_readFile_not_found(self):
         dir = self._makeOne()
-        self.assertRaises(IOError, dir.readFile, 'baz')
+        self.assertRaises(IOError, dir.readFile, "baz")
 
     def test_listDirectory(self):
         dir = self._makeOne()
-        self.assertEqual(['demo'], dir.listDirectory())
+        self.assertEqual(["demo"], dir.listDirectory())
 
     def test_listDirectory_filters_by_name(self):
         dir = self._makeOne()
-        dir.context._setOb('.svn', BTreeFolder2('filtered'))
-        self.assertEqual(['demo'], dir.listDirectory())
+        dir.context._setOb(".svn", BTreeFolder2("filtered"))
+        self.assertEqual(["demo"], dir.listDirectory())
 
     def test_makeDirectory(self):
         dir = self._makeOne()
-        dir.makeDirectory('demo/bar')
-        newdir = dir['demo']['bar']
+        dir.makeDirectory("demo/bar")
+        newdir = dir["demo"]["bar"]
         self.assertTrue(isinstance(newdir.context, BTreeFolder2))
 
     def test_makeDirectory_extra_slashes(self):
         dir = self._makeOne()
-        dir.makeDirectory('/demo/bar/')
-        newdir = dir['demo']['bar']
+        dir.makeDirectory("/demo/bar/")
+        newdir = dir["demo"]["bar"]
         self.assertTrue(isinstance(newdir.context, BTreeFolder2))
 
     def test_writeFile(self):
         dir = self._makeOne()
-        dir.writeFile('qux', b'qux')
-        self.assertEqual(b'qux', dir.readFile('qux'))
+        dir.writeFile("qux", b"qux")
+        self.assertEqual(b"qux", dir.readFile("qux"))
 
     def test_writeFile_does_not_create_empty_directory(self):
         dir = self._makeOne()
-        dir.writeFile('qux', b'qux')
-        self.assertFalse('' in dir)
-        self.assertTrue('qux' in dir)
+        dir.writeFile("qux", b"qux")
+        self.assertFalse("" in dir)
+        self.assertTrue("qux" in dir)
 
     def test_writeFile_directory_missing(self):
         dir = self._makeOne()
-        dir.writeFile('baz/qux', b'qux')
-        self.assertEqual(b'qux', dir.readFile('baz/qux'))
+        dir.writeFile("baz/qux", b"qux")
+        self.assertEqual(b"qux", dir.readFile("baz/qux"))
 
     def test_writeFile_file_already_exists(self):
         dir = self._makeOne()
-        dir.writeFile('demo/foo/test.html', b'changed')
-        self.assertEqual(b'changed', dir.readFile('demo/foo/test.html'))
+        dir.writeFile("demo/foo/test.html", b"changed")
+        self.assertEqual(b"changed", dir.readFile("demo/foo/test.html"))
 
     def test_importZip(self):
         dir = self._makeOne()
         with open(
-            os.path.join(os.path.dirname(__file__), 'resources.zip'),
-            'rb',
+            os.path.join(os.path.dirname(__file__), "resources.zip"),
+            "rb",
         ) as f:
             dir.importZip(f)
-            self.assertEqual(b'from zip', dir.readFile('demo/foo/test.html'))
+            self.assertEqual(b"from zip", dir.readFile("demo/foo/test.html"))
 
     def test_importZip_takes_ZipFile(self):
         dir = self._makeOne()
         with open(
-            os.path.join(os.path.dirname(__file__), 'resources.zip'),
-            'rb',
+            os.path.join(os.path.dirname(__file__), "resources.zip"),
+            "rb",
         ) as f:
             dir.importZip(f)
-            self.assertEqual(b'from zip', dir.readFile('demo/foo/test.html'))
+            self.assertEqual(b"from zip", dir.readFile("demo/foo/test.html"))
 
     def test_importZip_filters_resource_forks(self):
         dir = self._makeOne()
         with open(
-            os.path.join(os.path.dirname(__file__), 'resources.zip'),
-            'rb',
+            os.path.join(os.path.dirname(__file__), "resources.zip"),
+            "rb",
         ) as f:
             dir.importZip(f)
-            self.assertFalse('__MACOSX' in dir.context.objectIds())
+            self.assertFalse("__MACOSX" in dir.context.objectIds())
 
     def test_importZip_filters_hidden_directories(self):
         dir = self._makeOne()
         with open(
-            os.path.join(os.path.dirname(__file__), 'resources.zip'),
-            'rb',
+            os.path.join(os.path.dirname(__file__), "resources.zip"),
+            "rb",
         ) as f:
             dir.importZip(f)
-            self.assertFalse('.svn' in dir)
+            self.assertFalse(".svn" in dir)
 
     def test_delitem(self):
         dir = self._makeOne()
-        dir.makeDirectory('demo')
-        self.assertTrue('demo' in dir)
-        del dir['demo']
-        self.assertFalse('demo' in dir)
+        dir.makeDirectory("demo")
+        self.assertTrue("demo" in dir)
+        del dir["demo"]
+        self.assertFalse("demo" in dir)
 
     def test_rename(self):
         dir = self._makeOne()
-        dir.rename('demo', 'demo1')
-        self.assertEqual(['demo1'], dir.listDirectory())
+        dir.rename("demo", "demo1")
+        self.assertEqual(["demo1"], dir.listDirectory())
 
     def test_setitem_file(self):
         dir = self._makeOne()
-        f = dir['demo']['foo']['test.html']
-        dir['demo'].makeDirectory('bar')
+        f = dir["demo"]["foo"]["test.html"]
+        dir["demo"].makeDirectory("bar")
 
-        dir['demo']['bar']['test.html'] = f
-        self.assertEqual(dir['demo']['foo'].readFile('test.html'),
-                         dir['demo']['bar'].readFile('test.html'),)
+        dir["demo"]["bar"]["test.html"] = f
+        self.assertEqual(
+            dir["demo"]["foo"].readFile("test.html"),
+            dir["demo"]["bar"].readFile("test.html"),
+        )
 
     def test_setitem_file_unicode(self):
         dir = self._makeOne()
-        f = dir['demo']['foo']['test.html']
-        dir['demo'].makeDirectory('bar')
+        f = dir["demo"]["foo"]["test.html"]
+        dir["demo"].makeDirectory("bar")
 
-        dir['demo']['bar'][u'test.html'] = f
-        self.assertEqual(dir['demo']['foo'].readFile('test.html'),
-                         dir['demo']['bar'].readFile('test.html'),)
+        dir["demo"]["bar"]["test.html"] = f
+        self.assertEqual(
+            dir["demo"]["foo"].readFile("test.html"),
+            dir["demo"]["bar"].readFile("test.html"),
+        )
 
     def test_setitem_directory(self):
         dir = self._makeOne()
-        dir['demo']['foo'].makeDirectory('d1')
+        dir["demo"]["foo"].makeDirectory("d1")
 
-        d1 = dir['demo']['foo']['d1']
-        del dir['demo']['foo']['d1']
+        d1 = dir["demo"]["foo"]["d1"]
+        del dir["demo"]["foo"]["d1"]
 
-        dir['demo']['foo']['d2'] = d1
+        dir["demo"]["foo"]["d2"] = d1
 
-        self.assertEqual(dir['demo']['foo']['d2'].__name__, 'd2')
+        self.assertEqual(dir["demo"]["foo"]["d2"].__name__, "d2")
 
     def test_events(self):
         events = []
 
         @adapter(IPloneResourceCreatedEvent)
         def _handleFileCreated(event):
             events.append(event)
+
         provideHandler(_handleFileCreated)
 
         @adapter(IPloneResourceModifiedEvent)
         def _handleFileModified(event):
             events.append(event)
+
         provideHandler(_handleFileModified)
 
         dir = self._makeOne()
-        dir.writeFile('test', b'my test')
-        dir.writeFile('test', b'my test is modified')
+        dir.writeFile("test", b"my test")
+        dir.writeFile("test", b"my test is modified")
         self.assertTrue(isinstance(events[0], PloneResourceCreatedEvent))
-        self.assertEqual(events[0].object.data, b'my test')
+        self.assertEqual(events[0].object.data, b"my test")
         self.assertTrue(isinstance(events[1], PloneResourceModifiedEvent))
-        self.assertEqual(events[1].object.data, b'my test is modified')
+        self.assertEqual(events[1].object.data, b"my test is modified")
 
 
 class TestFilesystemResourceDirectory(unittest.TestCase):
-
     def _makeOne(self, name=None):
-        path = os.path.join(os.path.dirname(__file__), 'resources')
+        path = os.path.join(os.path.dirname(__file__), "resources")
         return FilesystemResourceDirectory(path, name=name)
 
     def test_repr_default(self):
         dir = self._makeOne()
-        s = '<FilesystemResourceDirectory object at resources>'
+        s = "<FilesystemResourceDirectory object at resources>"
         self.assertEqual(s, repr(dir))
 
     def test_repr_other_name(self):
-        dir = self._makeOne(name='something-else')
-        s = '<FilesystemResourceDirectory object at something-else>'
+        dir = self._makeOne(name="something-else")
+        s = "<FilesystemResourceDirectory object at something-else>"
         # This used to give a ValueError: substring not found
         self.assertEqual(s, repr(dir))
 
     def test_publishTraverse_directory(self):
         dir = self._makeOne()
-        subdir = dir.publishTraverse(None, 'demo')
-        self.assertEqual(subdir.directory, os.path.join(dir.directory, 'demo'))
+        subdir = dir.publishTraverse(None, "demo")
+        self.assertEqual(subdir.directory, os.path.join(dir.directory, "demo"))
 
     def test_publishTraverse_file(self):
         dir = self._makeOne()
-        file = dir.publishTraverse(None, 'demo/foo/test.html')
-        subpath = os.path.join(dir.directory, 'demo', 'foo', 'test.html')
+        file = dir.publishTraverse(None, "demo/foo/test.html")
+        subpath = os.path.join(dir.directory, "demo", "foo", "test.html")
         self.assertEqual(file.path, subpath)
 
     def test_publishTraverse_not_found(self):
         dir = self._makeOne()
-        self.assertRaises(NotFound, dir.publishTraverse, None, 'baz')
+        self.assertRaises(NotFound, dir.publishTraverse, None, "baz")
 
     def test_getitem(self):
         dir = self._makeOne()
-        subpath = os.path.join(dir.directory, 'demo')
-        self.assertEqual(dir['demo'].directory, subpath)
+        subpath = os.path.join(dir.directory, "demo")
+        self.assertEqual(dir["demo"].directory, subpath)
 
     def test_contains(self):
         dir = self._makeOne()
-        self.assertTrue('demo' in dir)
+        self.assertTrue("demo" in dir)
 
     def test_openFile(self):
         dir = self._makeOne()
-        with dir.openFile('demo/foo/test.html') as fp:
-            self.assertEqual(b'asdf', fp.read())
+        with dir.openFile("demo/foo/test.html") as fp:
+            self.assertEqual(b"asdf", fp.read())
 
     def test_readFile(self):
         dir = self._makeOne()
-        self.assertEqual(b'asdf', dir.readFile('demo/foo/test.html'))
+        self.assertEqual(b"asdf", dir.readFile("demo/foo/test.html"))
 
     def test_readFile_not_found(self):
         dir = self._makeOne()
-        self.assertRaises(IOError, dir.readFile, 'baz')
+        self.assertRaises(IOError, dir.readFile, "baz")
 
     def test_listDirectory(self):
         dir = self._makeOne()
-        self.assertEqual(['demo'], dir.listDirectory())
+        self.assertEqual(["demo"], dir.listDirectory())
 
     def test_listDirectory_filters_by_name(self):
         dir = self._makeOne()
-        name = '.dummy'
+        name = ".dummy"
         file_path = os.path.join(dir.directory, name)
         if name not in os.listdir(dir.directory):
-            with open(file_path, 'w') as fp:
+            with open(file_path, "w") as fp:
                 fp.write("")
         self.assertTrue(name in os.listdir(dir.directory))
-        self.assertEqual(['demo'], dir.listDirectory())
+        self.assertEqual(["demo"], dir.listDirectory())
         # Cleanup created file.
         os.remove(file_path)
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_file.py` & `plone.resource-3.0.0/plone/resource/tests/test_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,67 @@
-# -*- coding: utf-8 -*-
 from dateutil.tz import tzlocal
 from email.utils import formatdate
 from plone.resource.file import FileLastModified
 from plone.resource.file import FilesystemFile
 from plone.resource.file import rawReadFile
 from plone.testing.zca import UNIT_TESTING
 from z3c.caching.interfaces import ILastModified
 from zope.component import provideAdapter
 from zope.filerepresentation.interfaces import IRawReadFile
 from zope.publisher.browser import TestRequest
 
 import datetime
 import io
 import os.path
-import six
 import unittest
 
 
 class TestFilesystemResourceDirectory(unittest.TestCase):
-
     layer = UNIT_TESTING
 
     def test_render(self):
-        name = 'test.html'
-        path = os.path.join(os.path.dirname(__file__), 'resources', 'demo', 'foo', name)
+        name = "test.html"
+        path = os.path.join(os.path.dirname(__file__), "resources", "demo", "foo", name)
         mtime = os.path.getmtime(path)
 
         request = TestRequest()
 
         f = FilesystemFile(None, request, path, name)
         with f() as iterator:
-            data = b''.join(iterator)
-            self.assertEqual(data, b'asdf')
-            self.assertEqual(request.response.getHeader('Content-Type'), 'text/html')
-            self.assertEqual(request.response.getHeader('Content-Length'), '4')
-            self.assertEqual(request.response.getHeader('Last-Modified'), formatdate(mtime, usegmt=True))
+            data = b"".join(iterator)
+            self.assertEqual(data, b"asdf")
+            self.assertEqual(request.response.getHeader("Content-Type"), "text/html")
+            self.assertEqual(request.response.getHeader("Content-Length"), "4")
+            self.assertEqual(
+                request.response.getHeader("Last-Modified"),
+                formatdate(mtime, usegmt=True),
+            )
 
     def test_last_modified(self):
         provideAdapter(FileLastModified)
 
-        name = 'test.html'
-        path = os.path.join(os.path.dirname(__file__), 'resources', 'demo', 'foo', name)
+        name = "test.html"
+        path = os.path.join(os.path.dirname(__file__), "resources", "demo", "foo", name)
         mtime = os.path.getmtime(path)
 
         request = TestRequest()
 
         f = FilesystemFile(None, request, path, name)
 
         lastModified = ILastModified(f)
         mdate = datetime.datetime.fromtimestamp(mtime, tz=tzlocal())
 
         self.assertEqual(lastModified(), mdate)
 
     def test_raw_read_file(self):
         provideAdapter(rawReadFile)
 
-        name = 'test.html'
-        path = os.path.join(os.path.dirname(__file__), 'resources', 'demo', 'foo', name)
+        name = "test.html"
+        path = os.path.join(os.path.dirname(__file__), "resources", "demo", "foo", name)
 
         request = TestRequest()
 
         f = FilesystemFile(None, request, path, name)
 
         with IRawReadFile(f) as rf:
-            if six.PY2:
-                self.assertTrue(isinstance(rf, file))
-            else:
-                self.assertTrue(isinstance(rf, io.IOBase))
-            self.assertEqual(rf.read(), b'asdf')
+            self.assertTrue(isinstance(rf, io.IOBase))
+            self.assertEqual(rf.read(), b"asdf")
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_integration.py` & `plone.resource-3.0.0/plone/resource/tests/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# -*- coding: utf-8 -*-
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.testing import PLONE_RESOURCE_INTEGRATION_TESTING
 
 import unittest
 
 
 class IntegrationTestCase(unittest.TestCase):
     layer = PLONE_RESOURCE_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer.get('portal')
+        self.portal = self.layer.get("portal")
 
     def test_persistent_directory_installed(self):
         # directory should be available as the portal_resources tool
         from Products.CMFCore.utils import getToolByName
-        tool = getToolByName(self.portal, 'portal_resources')
-        self.assertEqual('portal_resources', tool.getId())
+
+        tool = getToolByName(self.portal, "portal_resources")
+        self.assertEqual("portal_resources", tool.getId())
 
         # wrapper should be available as an IResourceDirectory utility named 'persistent'
         from zope.component import getUtility
-        utility = getUtility(IResourceDirectory, name='persistent')
+
+        utility = getUtility(IResourceDirectory, name="persistent")
 
         # the utility's context attribute is the (unwrapped) tool
         from Acquisition import aq_base
+
         self.assertTrue(aq_base(tool) is utility.context)
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_manifest.py` & `plone.resource-3.0.0/plone/resource/tests/test_manifest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.directory import PersistentResourceDirectory
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.manifest import extractManifestFromZipFile
 from plone.resource.manifest import getAllResources
 from plone.resource.manifest import getManifest
 from plone.resource.manifest import getZODBResources
@@ -14,202 +13,243 @@
 
 import os.path
 import unittest
 import zipfile
 
 
 base_path = os.path.dirname(__file__)
-test_dir_path = os.path.join(base_path, 'resources')
+test_dir_path = os.path.join(base_path, "resources")
+
+TEST_FORMAT = ManifestFormat("demo", ["title", "description", "bar"], {"bar": "baz"})
+TEST_FORMAT_PARAMS = ManifestFormat(
+    "demo", ["title", "description", "bar"], {"bar": "baz"}, ["params"]
+)
 
-TEST_FORMAT = ManifestFormat('demo', ['title', 'description', 'bar'], {'bar': 'baz'})
-TEST_FORMAT_PARAMS = ManifestFormat('demo', ['title', 'description', 'bar'], {'bar': 'baz'}, ['params'])
 
 class TestManifest(unittest.TestCase):
     layer = DEMO_TRAVERSER_FUNCTIONAL_TESTING
 
     def setUp(self):
         zca.pushGlobalRegistry()
 
     def tearDown(self):
         zca.popGlobalRegistry()
 
     def test_get_manifest(self):
-        with open(os.path.join(test_dir_path, 'demo', 'manifest-test', 'manifest.cfg')) as fp:
+        with open(
+            os.path.join(test_dir_path, "demo", "manifest-test", "manifest.cfg")
+        ) as fp:
             manifest = getManifest(fp, TEST_FORMAT)
-            self.assertEqual(manifest['title'], 'Manifest test')
-            self.assertEqual(manifest['description'], None)
-            self.assertEqual(manifest['bar'], 'baz')
+            self.assertEqual(manifest["title"], "Manifest test")
+            self.assertEqual(manifest["description"], None)
+            self.assertEqual(manifest["bar"], "baz")
 
     def test_get_manifest_params(self):
-        with open(os.path.join(test_dir_path, 'demo', 'manifest-test', 'manifest.cfg')) as fp:
+        with open(
+            os.path.join(test_dir_path, "demo", "manifest-test", "manifest.cfg")
+        ) as fp:
             manifest = getManifest(fp, TEST_FORMAT_PARAMS)
-            self.assertEqual(manifest['title'], 'Manifest test')
-            self.assertEqual(manifest['description'], None)
-            self.assertEqual(manifest['bar'], 'baz')
-            self.assertEqual(manifest['params'], {'alpha': 'beta', 'delta': 'theta'})
+            self.assertEqual(manifest["title"], "Manifest test")
+            self.assertEqual(manifest["description"], None)
+            self.assertEqual(manifest["bar"], "baz")
+            self.assertEqual(manifest["params"], {"alpha": "beta", "delta": "theta"})
 
     def test_get_manifest_ignores_extra(self):
-        with open(os.path.join(test_dir_path, 'demo', 'manifest-test', 'manifest.cfg')) as fp:
+        with open(
+            os.path.join(test_dir_path, "demo", "manifest-test", "manifest.cfg")
+        ) as fp:
             manifest = getManifest(fp, TEST_FORMAT)
-            self.assertFalse('baz' in manifest)
+            self.assertFalse("baz" in manifest)
 
     def test_get_manifest_override_defaults(self):
-        with open(os.path.join(test_dir_path, 'demo', 'manifest-test', 'manifest.cfg')) as fp:
-            manifest = getManifest(fp, TEST_FORMAT, {'bar': 'foo', 'title': 'foo'})
-            self.assertEqual(manifest['title'], 'Manifest test')
-            self.assertEqual(manifest['bar'], 'foo')
+        with open(
+            os.path.join(test_dir_path, "demo", "manifest-test", "manifest.cfg")
+        ) as fp:
+            manifest = getManifest(fp, TEST_FORMAT, {"bar": "foo", "title": "foo"})
+            self.assertEqual(manifest["title"], "Manifest test")
+            self.assertEqual(manifest["bar"], "foo")
 
     def test_extract_from_zip_file(self):
-        zf = zipfile.ZipFile(os.path.join(base_path, 'zipfiles', 'normal.zip'))
+        zf = zipfile.ZipFile(os.path.join(base_path, "zipfiles", "normal.zip"))
         resourceName, manifestDict = extractManifestFromZipFile(zf, TEST_FORMAT)
 
-        self.assertEqual(resourceName, 'demo1')
+        self.assertEqual(resourceName, "demo1")
         self.assertEqual(
-                manifestDict,
-                {'bar': 'baz', 'description': None, 'title': 'No top level dir'}
-            )
+            manifestDict,
+            {"bar": "baz", "description": None, "title": "No top level dir"},
+        )
 
     def test_extract_from_zip_file_override_defaults(self):
-        zf = zipfile.ZipFile(os.path.join(base_path, 'zipfiles', 'normal.zip'))
-        resourceName, manifestDict = extractManifestFromZipFile(zf, TEST_FORMAT,
-            defaults={'bar': 'foo', 'description': 'desc'})
-
-        self.assertEqual(resourceName, 'demo1')
-        self.assertEqual(
-                manifestDict,
-                {'bar': 'foo', 'description': 'desc', 'title': 'No top level dir'}
-            )
+        zf = zipfile.ZipFile(os.path.join(base_path, "zipfiles", "normal.zip"))
+        resourceName, manifestDict = extractManifestFromZipFile(
+            zf, TEST_FORMAT, defaults={"bar": "foo", "description": "desc"}
+        )
+
+        self.assertEqual(resourceName, "demo1")
+        self.assertEqual(
+            manifestDict,
+            {"bar": "foo", "description": "desc", "title": "No top level dir"},
+        )
 
     def test_extract_from_zip_file_no_top_level_dir(self):
-        zf = zipfile.ZipFile(os.path.join(base_path, 'zipfiles', 'no-top-level-dir.zip'))
+        zf = zipfile.ZipFile(
+            os.path.join(base_path, "zipfiles", "no-top-level-dir.zip")
+        )
         self.assertRaises(ValueError, extractManifestFromZipFile, zf, TEST_FORMAT)
 
     def test_extract_from_zip_file_multiple_top_level_dirs(self):
-        zf = zipfile.ZipFile(os.path.join(base_path, 'zipfiles', 'multiple-top-level-dirs.zip'))
+        zf = zipfile.ZipFile(
+            os.path.join(base_path, "zipfiles", "multiple-top-level-dirs.zip")
+        )
         self.assertRaises(ValueError, extractManifestFromZipFile, zf, TEST_FORMAT)
 
     def test_extract_from_zip_file_no_manifest(self):
-        zf = zipfile.ZipFile(os.path.join(base_path, 'zipfiles', 'no-manifest.zip'))
+        zf = zipfile.ZipFile(os.path.join(base_path, "zipfiles", "no-manifest.zip"))
         resourceName, manifestDict = extractManifestFromZipFile(zf, TEST_FORMAT)
 
-        self.assertEqual(resourceName, 'demo1')
+        self.assertEqual(resourceName, "demo1")
         self.assertEqual(manifestDict, None)
 
     def test_extract_from_zip_file_manifest_name_override(self):
-        zf = zipfile.ZipFile(os.path.join(base_path, 'zipfiles', 'manifest-name-override.zip'))
+        zf = zipfile.ZipFile(
+            os.path.join(base_path, "zipfiles", "manifest-name-override.zip")
+        )
         resourceName, manifestDict = extractManifestFromZipFile(zf, TEST_FORMAT)
 
-        self.assertEqual(resourceName, 'demo1')
+        self.assertEqual(resourceName, "demo1")
         self.assertEqual(manifestDict, None)
 
-        resourceName, manifestDict = extractManifestFromZipFile(zf, TEST_FORMAT, manifestFilename='other-manifest.cfg')
+        resourceName, manifestDict = extractManifestFromZipFile(
+            zf, TEST_FORMAT, manifestFilename="other-manifest.cfg"
+        )
 
         self.assertEqual(
-                manifestDict,
-                {'bar': 'baz', 'description': None, 'title': 'No top level dir'}
-            )
+            manifestDict,
+            {"bar": "baz", "description": None, "title": "No top level dir"},
+        )
 
     def test_get_all_resources(self):
-        app = self.layer['app']
+        app = self.layer["app"]
 
-        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'foo'))
-        provideUtility(foo, provides=IResourceDirectory, name=u'++demo++foo')
+        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, "demo", "foo"))
+        provideUtility(foo, provides=IResourceDirectory, name="++demo++foo")
 
-        manifestTest = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'manifest-test'))
-        provideUtility(manifestTest, provides=IResourceDirectory, name=u'++demo++manifest-test')
-
-        root = BTreeFolder2('portal_resources')
-        app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root['demo']._setOb('bar', BTreeFolder2('bar'))
+        manifestTest = FilesystemResourceDirectory(
+            os.path.join(test_dir_path, "demo", "manifest-test")
+        )
+        provideUtility(
+            manifestTest, provides=IResourceDirectory, name="++demo++manifest-test"
+        )
+
+        root = BTreeFolder2("portal_resources")
+        app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root["demo"]._setOb("bar", BTreeFolder2("bar"))
 
         persistentDir = PersistentResourceDirectory(root)
-        provideUtility(persistentDir, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(persistentDir, provides=IResourceDirectory, name="persistent")
 
         resources = getAllResources(TEST_FORMAT)
 
         self.assertEqual(
-                resources,
-                {'bar': None,
-                 'foo': None,
-                 'manifest-test': {'bar': 'baz',
-                                   'description': None,
-                                   'title': 'Manifest test'}}
-            )
+            resources,
+            {
+                "bar": None,
+                "foo": None,
+                "manifest-test": {
+                    "bar": "baz",
+                    "description": None,
+                    "title": "Manifest test",
+                },
+            },
+        )
 
     def test_get_all_resources_filter(self):
-        app = self.layer['app']
-
-        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'foo'))
-        provideUtility(foo, provides=IResourceDirectory, name=u'++demo++foo')
+        app = self.layer["app"]
 
-        manifestTest = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'manifest-test'))
-        provideUtility(manifestTest, provides=IResourceDirectory, name=u'++demo++manifest-test')
+        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, "demo", "foo"))
+        provideUtility(foo, provides=IResourceDirectory, name="++demo++foo")
 
-        root = BTreeFolder2('portal_resources')
-        app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root['demo']._setOb('bar', BTreeFolder2('bar'))
+        manifestTest = FilesystemResourceDirectory(
+            os.path.join(test_dir_path, "demo", "manifest-test")
+        )
+        provideUtility(
+            manifestTest, provides=IResourceDirectory, name="++demo++manifest-test"
+        )
+
+        root = BTreeFolder2("portal_resources")
+        app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root["demo"]._setOb("bar", BTreeFolder2("bar"))
 
         persistentDir = PersistentResourceDirectory(root)
-        provideUtility(persistentDir, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(persistentDir, provides=IResourceDirectory, name="persistent")
 
-        resources = getAllResources(TEST_FORMAT, filter=lambda dir: dir.__name__ != 'foo')
-
-        self.assertEqual(
-                resources,
-                {'bar': None,
-                 'manifest-test': {'bar': 'baz',
-                                   'description': None,
-                                   'title': 'Manifest test'}}
-            )
+        resources = getAllResources(
+            TEST_FORMAT, filter=lambda dir: dir.__name__ != "foo"
+        )
+
+        self.assertEqual(
+            resources,
+            {
+                "bar": None,
+                "manifest-test": {
+                    "bar": "baz",
+                    "description": None,
+                    "title": "Manifest test",
+                },
+            },
+        )
 
     def test_get_zodb_resources(self):
-        app = self.layer['app']
-
-        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'foo'))
-        provideUtility(foo, provides=IResourceDirectory, name=u'++demo++foo')
+        app = self.layer["app"]
 
-        manifestTest = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'manifest-test'))
-        provideUtility(manifestTest, provides=IResourceDirectory, name=u'++demo++manifest-test')
+        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, "demo", "foo"))
+        provideUtility(foo, provides=IResourceDirectory, name="++demo++foo")
 
-        root = BTreeFolder2('portal_resources')
-        app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root['demo']._setOb('bar', BTreeFolder2('bar'))
-        root['demo']._setOb('baz', BTreeFolder2('baz'))
+        manifestTest = FilesystemResourceDirectory(
+            os.path.join(test_dir_path, "demo", "manifest-test")
+        )
+        provideUtility(
+            manifestTest, provides=IResourceDirectory, name="++demo++manifest-test"
+        )
+
+        root = BTreeFolder2("portal_resources")
+        app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root["demo"]._setOb("bar", BTreeFolder2("bar"))
+        root["demo"]._setOb("baz", BTreeFolder2("baz"))
 
         persistentDir = PersistentResourceDirectory(root)
-        provideUtility(persistentDir, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(persistentDir, provides=IResourceDirectory, name="persistent")
 
         resources = getZODBResources(TEST_FORMAT)
 
-        self.assertEqual(
-                resources,
-                {'bar': None,
-                 'baz': None}
-            )
+        self.assertEqual(resources, {"bar": None, "baz": None})
 
     def test_get_zodb_resources_filter(self):
-        app = self.layer['app']
+        app = self.layer["app"]
 
-        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'foo'))
-        provideUtility(foo, provides=IResourceDirectory, name=u'++demo++foo')
+        foo = FilesystemResourceDirectory(os.path.join(test_dir_path, "demo", "foo"))
+        provideUtility(foo, provides=IResourceDirectory, name="++demo++foo")
 
-        manifestTest = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'manifest-test'))
-        provideUtility(manifestTest, provides=IResourceDirectory, name=u'++demo++manifest-test')
-
-        root = BTreeFolder2('portal_resources')
-        app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root['demo']._setOb('bar', BTreeFolder2('bar'))
-        root['demo']._setOb('baz', BTreeFolder2('baz'))
+        manifestTest = FilesystemResourceDirectory(
+            os.path.join(test_dir_path, "demo", "manifest-test")
+        )
+        provideUtility(
+            manifestTest, provides=IResourceDirectory, name="++demo++manifest-test"
+        )
+
+        root = BTreeFolder2("portal_resources")
+        app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root["demo"]._setOb("bar", BTreeFolder2("bar"))
+        root["demo"]._setOb("baz", BTreeFolder2("baz"))
 
         persistentDir = PersistentResourceDirectory(root)
-        provideUtility(persistentDir, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(persistentDir, provides=IResourceDirectory, name="persistent")
 
-        resources = getZODBResources(TEST_FORMAT, filter=lambda dir: dir.__name__ != 'baz')
+        resources = getZODBResources(
+            TEST_FORMAT, filter=lambda dir: dir.__name__ != "baz"
+        )
 
-        self.assertEqual(
-                resources,
-                {'bar': None}
-            )
+        self.assertEqual(resources, {"bar": None})
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_traversal.py` & `plone.resource-3.0.0/plone/resource/tests/test_traversal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,116 +1,111 @@
-# -*- coding: utf-8 -*-
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.directory import PersistentResourceDirectory
 from plone.resource.file import FilesystemFile
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.interfaces import IUniqueResourceRequest
 from plone.resource.testing import DEMO_TRAVERSER_FUNCTIONAL_TESTING
-from plone.testing import zope
 from plone.testing import zca
+from plone.testing import zope
 from Products.BTreeFolder2.BTreeFolder2 import BTreeFolder2
 from zExceptions import Forbidden
 from zExceptions import NotFound
 from zope.component import provideUtility
 
 import os.path
 import unittest
 
 
 base_path = os.path.dirname(__file__)
-test_dir_path = os.path.join(base_path, 'resources')
+test_dir_path = os.path.join(base_path, "resources")
 
 
 class TraversalTestCase(unittest.TestCase):
     layer = DEMO_TRAVERSER_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.app = self.layer.get('app')
+        self.app = self.layer.get("app")
         zca.pushGlobalRegistry()
 
     def tearDown(self):
         zca.popGlobalRegistry()
 
     def test_traverse_packaged_type_specific_directory(self):
         dire = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dire, provides=IResourceDirectory, name=u'++demo++foo')
+        provideUtility(dire, provides=IResourceDirectory, name="++demo++foo")
 
-        res = self.app.restrictedTraverse('++demo++foo')
-        self.assertTrue(res.directory.endswith('resources'))
+        res = self.app.restrictedTraverse("++demo++foo")
+        self.assertTrue(res.directory.endswith("resources"))
 
         self.assertRaises(
             NotFound,
             self.app.restrictedTraverse,
-            '++demo++asdf',
+            "++demo++asdf",
         )
 
     def test_traverse_packaged_type_specific_file(self):
-        dire = FilesystemResourceDirectory(
-            os.path.join(test_dir_path, 'demo', 'foo')
-        )
-        provideUtility(dire, provides=IResourceDirectory, name=u'++demo++foo')
+        dire = FilesystemResourceDirectory(os.path.join(test_dir_path, "demo", "foo"))
+        provideUtility(dire, provides=IResourceDirectory, name="++demo++foo")
 
-        res = self.app.restrictedTraverse('++demo++foo/test.html')
+        res = self.app.restrictedTraverse("++demo++foo/test.html")
         self.assertTrue(isinstance(res, FilesystemFile))
 
     def test_traverse_global_directory(self):
         dire = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dire, provides=IResourceDirectory, name=u'')
+        provideUtility(dire, provides=IResourceDirectory, name="")
 
-        res = self.app.restrictedTraverse('++demo++foo')
-        self.assertTrue(res.directory.endswith('resources/demo/foo'))
+        res = self.app.restrictedTraverse("++demo++foo")
+        self.assertTrue(res.directory.endswith("resources/demo/foo"))
 
-        self.assertRaises(NotFound, self.app.restrictedTraverse, '++demo++bar')
+        self.assertRaises(NotFound, self.app.restrictedTraverse, "++demo++bar")
 
     def test_traverse_persistent_directory(self):
-        root = BTreeFolder2('portal_resources')
-        self.app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root.demo._setOb('foo', BTreeFolder2('foo'))
+        root = BTreeFolder2("portal_resources")
+        self.app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root.demo._setOb("foo", BTreeFolder2("foo"))
 
         dire = PersistentResourceDirectory(root)
-        provideUtility(dire, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(dire, provides=IResourceDirectory, name="persistent")
 
-        res = self.app.restrictedTraverse('++demo++foo')
+        res = self.app.restrictedTraverse("++demo++foo")
         self.assertEqual(
-            'portal_resources/demo/foo', '/'.join(
+            "portal_resources/demo/foo",
+            "/".join(
                 res.context.getPhysicalPath(),
             ),
         )
 
-        self.assertRaises(NotFound, self.app.restrictedTraverse, '++demo++bar')
+        self.assertRaises(NotFound, self.app.restrictedTraverse, "++demo++bar")
 
     def test_publish_resource(self):
         dire = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dire, provides=IResourceDirectory, name=u'')
+        provideUtility(dire, provides=IResourceDirectory, name="")
 
         browser = zope.Browser(self.app)
         browser.handleErrors = False
 
-        browser.open(self.app.absolute_url() + '/++demo++foo/test.html')
-        self.assertEqual('asdf', browser.contents)
+        browser.open(self.app.absolute_url() + "/++demo++foo/test.html")
+        self.assertEqual("asdf", browser.contents)
 
     def test_traverse_unique_resource_marks_request(self):
         dire = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dire, provides=IResourceDirectory, name=u'')
+        provideUtility(dire, provides=IResourceDirectory, name="")
 
-        self.app.restrictedTraverse(
-            '++demo++foo/++unique++bar/test.html'
-        )
+        self.app.restrictedTraverse("++demo++foo/++unique++bar/test.html")
         self.assertTrue(IUniqueResourceRequest.providedBy(self.app.REQUEST))
 
     def test_publish_unique_resource(self):
         dire = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dire, provides=IResourceDirectory, name=u'')
+        provideUtility(dire, provides=IResourceDirectory, name="")
 
         browser = zope.Browser(self.app)
         browser.handleErrors = False
 
-        browser.open(
-            self.app.absolute_url() + '/++demo++foo/++unique++bar/test.html'
-        )
-        self.assertEqual('asdf', browser.contents)
+        browser.open(self.app.absolute_url() + "/++demo++foo/++unique++bar/test.html")
+        self.assertEqual("asdf", browser.contents)
 
     def test_forbidden_resource_path_traversal(self):
         resource_directory = FilesystemResourceDirectory(test_dir_path)
-        self.assertRaises(Forbidden, resource_directory._resolveSubpath,
-                          '../../../../setup.py')
+        self.assertRaises(
+            Forbidden, resource_directory._resolveSubpath, "../../../../setup.py"
+        )
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_utils.py` & `plone.resource-3.0.0/plone/resource/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,102 @@
-# -*- coding: utf-8 -*-
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.directory import PersistentResourceDirectory
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.testing import DEMO_TRAVERSER_FUNCTIONAL_TESTING
 from plone.testing import zca
 from Products.BTreeFolder2.BTreeFolder2 import BTreeFolder2
 from zope.component import provideUtility
 
 import os.path
 import unittest
 
 
 base_path = os.path.dirname(__file__)
-test_dir_path = os.path.join(base_path, 'resources')
+test_dir_path = os.path.join(base_path, "resources")
 
 
 class TraversalTestCase(unittest.TestCase):
     layer = DEMO_TRAVERSER_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.app = self.layer.get('app')
+        self.app = self.layer.get("app")
         zca.pushGlobalRegistry()
 
         # set up all three types of directory
-        package_dir_path = os.path.join(test_dir_path, 'demo', 'foo')
+        package_dir_path = os.path.join(test_dir_path, "demo", "foo")
         self.package_dir = dir = FilesystemResourceDirectory(package_dir_path)
-        provideUtility(dir, provides=IResourceDirectory, name=u'++demo++foo')
+        provideUtility(dir, provides=IResourceDirectory, name="++demo++foo")
 
         self.global_dir = dir = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dir, provides=IResourceDirectory, name=u'')
+        provideUtility(dir, provides=IResourceDirectory, name="")
 
-        root = BTreeFolder2('portal_resources')
-        self.app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root.demo._setOb('foo', BTreeFolder2('foo'))
+        root = BTreeFolder2("portal_resources")
+        self.app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root.demo._setOb("foo", BTreeFolder2("foo"))
         self.zodb_dir = dir = PersistentResourceDirectory(root)
-        provideUtility(dir, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(dir, provides=IResourceDirectory, name="persistent")
 
         # We don't want a false positive for the following.
-        provideUtility(dir, provides=IResourceDirectory, name=u'++bogus++foo')
+        provideUtility(dir, provides=IResourceDirectory, name="++bogus++foo")
 
     def tearDown(self):
         zca.popGlobalRegistry()
 
     def test_iterDirectoriesOfType(self):
         from plone.resource.utils import iterDirectoriesOfType
-        dirs = list(iterDirectoriesOfType('demo'))
+
+        dirs = list(iterDirectoriesOfType("demo"))
         self.assertEqual(2, len(dirs))
-        self.assertTrue(dirs[0].context.aq_base is
-                        self.zodb_dir['demo']['foo'].context.aq_base)
-        self.assertTrue(dirs[1].directory ==
-                        self.global_dir['demo']['manifest-test'].directory)
+        self.assertTrue(
+            dirs[0].context.aq_base is self.zodb_dir["demo"]["foo"].context.aq_base
+        )
+        self.assertTrue(
+            dirs[1].directory == self.global_dir["demo"]["manifest-test"].directory
+        )
 
     def test_iterDirectoriesOfType_dont_filter_duplicates(self):
         from plone.resource.utils import iterDirectoriesOfType
-        dirs = list(iterDirectoriesOfType('demo', filter_duplicates=False))
+
+        dirs = list(iterDirectoriesOfType("demo", filter_duplicates=False))
         self.assertEqual(4, len(dirs))
-        self.assertTrue(dirs[0].context.aq_base is
-                        self.zodb_dir['demo']['foo'].context.aq_base)
+        self.assertTrue(
+            dirs[0].context.aq_base is self.zodb_dir["demo"]["foo"].context.aq_base
+        )
         unordered_entries = [
-            self.global_dir['demo']['foo'].directory,
-            self.global_dir['demo']['manifest-test'].directory
+            self.global_dir["demo"]["foo"].directory,
+            self.global_dir["demo"]["manifest-test"].directory,
         ]
         self.assertIn(dirs[1].directory, unordered_entries)
         self.assertIn(dirs[2].directory, unordered_entries)
         self.assertNotEqual(dirs[1].directory, dirs[2].directory)
         self.assertTrue(dirs[3].directory == self.package_dir.directory)
 
     def test_cloneDirectory(self):
         from plone.resource.directory import PersistentResourceDirectory
         from plone.resource.utils import cloneResourceDirectory
 
-        root = BTreeFolder2('portal_resources')
-        root._setOb('demo', BTreeFolder2('demo'))
-        root['demo']._setOb('foo', BTreeFolder2('foo'))
-        root['demo']._setOb('bar', BTreeFolder2('bar'))
-
-        source = PersistentResourceDirectory(root['demo']['foo'])
-        target = PersistentResourceDirectory(root['demo']['bar'])
-
-        source.writeFile('file1.txt', b'file1')
-        source.writeFile('subdir1/file2.txt', b'file2')
-        source.makeDirectory('subdir2')
+        root = BTreeFolder2("portal_resources")
+        root._setOb("demo", BTreeFolder2("demo"))
+        root["demo"]._setOb("foo", BTreeFolder2("foo"))
+        root["demo"]._setOb("bar", BTreeFolder2("bar"))
+
+        source = PersistentResourceDirectory(root["demo"]["foo"])
+        target = PersistentResourceDirectory(root["demo"]["bar"])
+
+        source.writeFile("file1.txt", b"file1")
+        source.writeFile("subdir1/file2.txt", b"file2")
+        source.makeDirectory("subdir2")
 
         cloneResourceDirectory(source, target)
 
         self.assertEqual(source.listDirectory(), target.listDirectory())
-        self.assertEqual(source['subdir1'].listDirectory(), target['subdir1'].listDirectory())
-        self.assertEqual(source['subdir2'].listDirectory(), target['subdir2'].listDirectory())
-        self.assertEqual(source.readFile('file1.txt'), target.readFile('file1.txt'))
-        self.assertEqual(source.readFile('subdir1/file2.txt'), target.readFile('subdir1/file2.txt'))
+        self.assertEqual(
+            source["subdir1"].listDirectory(), target["subdir1"].listDirectory()
+        )
+        self.assertEqual(
+            source["subdir2"].listDirectory(), target["subdir2"].listDirectory()
+        )
+        self.assertEqual(source.readFile("file1.txt"), target.readFile("file1.txt"))
+        self.assertEqual(
+            source.readFile("subdir1/file2.txt"), target.readFile("subdir1/file2.txt")
+        )
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_zcml.py` & `plone.resource-3.0.0/plone/resource/tests/test_zcml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,123 @@
-# -*- coding: utf-8 -*-
-import os.path
-import unittest
-
+from io import StringIO
 from plone.resource.interfaces import IResourceDirectory
-from six import StringIO
 from zope.component import getUtility
 from zope.component.testing import tearDown
 from zope.configuration.exceptions import ConfigurationError
-from zope.configuration.xmlconfig import XMLConfig, xmlconfig
+from zope.configuration.xmlconfig import XMLConfig
+from zope.configuration.xmlconfig import xmlconfig
+
+import os.path
+import unittest
 
 
 def clearZCML(test=None):
     # Copy from ``zope.component.tests.examples``
-    from zope.configuration.xmlconfig import XMLConfig
-    import zope.component
     from zope.component.testing import setUp
     from zope.component.testing import tearDown
+    from zope.configuration.xmlconfig import XMLConfig
+
+    import zope.component
+
     tearDown()
     setUp()
-    XMLConfig('meta.zcml', zope.component)()
+    XMLConfig("meta.zcml", zope.component)()
 
 
-def runSnippet(snippet, dist='plone.resource.tests'):
+def runSnippet(snippet, dist="plone.resource.tests"):
     template = """\
     <configure xmlns="http://namespaces.zope.org/zope"
                xmlns:plone="http://namespaces.plone.org/plone"
                i18n_domain="plone"
                %s>
     %s
     </configure>"""
-    dist = 'package="%s"' % dist if dist else ''
+    dist = 'package="%s"' % dist if dist else ""
     xmlconfig(StringIO(template % (dist, snippet)))
 
 
 class ZCMLTestCase(unittest.TestCase):
-
     def setUp(self):
         clearZCML()
         import plone.resource
-        XMLConfig('meta.zcml', plone.resource)()
+
+        XMLConfig("meta.zcml", plone.resource)()
 
     def tearDown(self):
         tearDown()
 
     def test_dist_with_name_and_type(self):
-        runSnippet("""
+        runSnippet(
+            """
         <plone:static
           name="foo"
           type="theme"
           directory="resources"
           />
-        """)
+        """
+        )
 
-        res = getUtility(IResourceDirectory, name='++theme++foo')
-        self.assertTrue(res.directory.endswith(os.path.join('plone', 'resource', 'tests', 'resources')))
+        res = getUtility(IResourceDirectory, name="++theme++foo")
+        self.assertTrue(
+            res.directory.endswith(
+                os.path.join("plone", "resource", "tests", "resources")
+            )
+        )
 
     def test_dist_rejects_with_missing_type(self):
         # resource directories in distributions must be registered with a type
-        self.assertRaises(ConfigurationError,
+        self.assertRaises(
+            ConfigurationError,
             runSnippet,
             """<plone:static
               name="foo"
               directory="resources"
-              />"""
-            )
+              />""",
+        )
 
     def test_dist_with_type_only(self):
-        runSnippet("""
+        runSnippet(
+            """
         <plone:static
           type="theme"
           directory="resources"
           />
-        """)
+        """
+        )
 
-        getUtility(IResourceDirectory, name='++theme++plone.resource.tests')
+        getUtility(IResourceDirectory, name="++theme++plone.resource.tests")
 
     def test_dist_rejects_absolute_directory(self):
-        self.assertRaises(ConfigurationError,
-            runSnippet,
-            """<plone:static directory="/" />"""
-            )
+        self.assertRaises(
+            ConfigurationError, runSnippet, """<plone:static directory="/" />"""
+        )
 
     def test_global(self):
-        runSnippet("""
+        runSnippet(
+            """
         <plone:static
           directory="/"
           />
-        """, dist=None)
+        """,
+            dist=None,
+        )
 
         res = getUtility(IResourceDirectory)
-        self.assertEqual('/', res.directory)
+        self.assertEqual("/", res.directory)
 
     def test_global_rejects_relative_directory(self):
-        self.assertRaises(ConfigurationError,
+        self.assertRaises(
+            ConfigurationError,
             runSnippet,
             """<plone:static directory="foobar" />""",
-            dist=None
-            )
+            dist=None,
+        )
 
     def test_missing_directory(self):
-        self.assertRaises(ConfigurationError,
-            runSnippet,
-            """<plone:static directory="foobar" />"""
-            )
+        self.assertRaises(
+            ConfigurationError, runSnippet, """<plone:static directory="foobar" />"""
+        )
 
     def test_rejects_parent_directory_traversal(self):
-        self.assertRaises(ConfigurationError,
-            runSnippet,
-            """<plone:static directory="../tests" />"""
-            )
+        self.assertRaises(
+            ConfigurationError, runSnippet, """<plone:static directory="../tests" />"""
+        )
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/test_zip_download.py` & `plone.resource-3.0.0/plone/resource/tests/test_zip_download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from io import BytesIO
 from OFS.Image import File
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.directory import PersistentResourceDirectory
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.testing import DEMO_TRAVERSER_FUNCTIONAL_TESTING
 from plone.testing import zca
@@ -11,79 +10,79 @@
 
 import os.path
 import unittest
 import zipfile
 
 
 base_path = os.path.dirname(__file__)
-test_dir_path = os.path.join(base_path, 'resources')
+test_dir_path = os.path.join(base_path, "resources")
 
 
 class ZipDownloadTestCase(unittest.TestCase):
     layer = DEMO_TRAVERSER_FUNCTIONAL_TESTING
 
     def setUp(self):
-        self.app = self.layer.get('app')
+        self.app = self.layer.get("app")
         zca.pushGlobalRegistry()
 
     def tearDown(self):
         zca.popGlobalRegistry()
 
     def test_traverse_packaged_type_specific_directory(self):
-        dir = FilesystemResourceDirectory(os.path.join(test_dir_path, 'demo', 'foo'))
-        provideUtility(dir, provides=IResourceDirectory, name=u'++demo++foo')
+        dir = FilesystemResourceDirectory(os.path.join(test_dir_path, "demo", "foo"))
+        provideUtility(dir, provides=IResourceDirectory, name="++demo++foo")
 
         out = BytesIO()
-        request = self.layer['request']
+        request = self.layer["request"]
         response = request.response
         response.stdout = out
 
-        zipview = self.app.unrestrictedTraverse('++demo++foo/@@download-zip')
+        zipview = self.app.unrestrictedTraverse("++demo++foo/@@download-zip")
         zipview()
 
         zf = zipfile.ZipFile(out)
 
-        self.assertTrue('foo/test.html' in zf.namelist())
-        self.assertEqual(b'asdf', zf.open('foo/test.html').read())
+        self.assertTrue("foo/test.html" in zf.namelist())
+        self.assertEqual(b"asdf", zf.open("foo/test.html").read())
 
     def test_traverse_global_directory(self):
         dir = FilesystemResourceDirectory(test_dir_path)
-        provideUtility(dir, provides=IResourceDirectory, name=u'')
+        provideUtility(dir, provides=IResourceDirectory, name="")
 
         out = BytesIO()
-        request = self.layer['request']
+        request = self.layer["request"]
         response = request.response
         response.stdout = out
 
-        zipview = self.app.unrestrictedTraverse('++demo++foo/@@download-zip')
+        zipview = self.app.unrestrictedTraverse("++demo++foo/@@download-zip")
         zipview()
 
         zf = zipfile.ZipFile(out)
 
-        self.assertTrue('foo/test.html' in zf.namelist())
-        self.assertEqual(b'asdf', zf.open('foo/test.html').read())
+        self.assertTrue("foo/test.html" in zf.namelist())
+        self.assertEqual(b"asdf", zf.open("foo/test.html").read())
 
     def test_traverse_persistent_directory(self):
-        root = BTreeFolder2('portal_resources')
-        self.app._setOb('portal_resources', root)
-        root._setOb('demo', BTreeFolder2('demo'))
-        root['demo']._setOb('foo', BTreeFolder2('foo'))
-        root['demo']['foo']._setOb(
-            'test.html',
-            File('test.html', 'test.html', b'asdf'),
+        root = BTreeFolder2("portal_resources")
+        self.app._setOb("portal_resources", root)
+        root._setOb("demo", BTreeFolder2("demo"))
+        root["demo"]._setOb("foo", BTreeFolder2("foo"))
+        root["demo"]["foo"]._setOb(
+            "test.html",
+            File("test.html", "test.html", b"asdf"),
         )
 
         dir = PersistentResourceDirectory(root)
-        provideUtility(dir, provides=IResourceDirectory, name=u'persistent')
+        provideUtility(dir, provides=IResourceDirectory, name="persistent")
 
         out = BytesIO()
-        request = self.layer['request']
+        request = self.layer["request"]
         response = request.response
         response.stdout = out
 
-        zipview = self.app.unrestrictedTraverse('++demo++foo/@@download-zip')
+        zipview = self.app.unrestrictedTraverse("++demo++foo/@@download-zip")
         zipview()
 
         zf = zipfile.ZipFile(out)
 
-        self.assertTrue('foo/test.html' in zf.namelist())
-        self.assertEqual(b'asdf', zf.open('foo/test.html').read())
+        self.assertTrue("foo/test.html" in zf.namelist())
+        self.assertEqual(b"asdf", zf.open("foo/test.html").read())
```

### Comparing `plone.resource-2.1.4/plone/resource/tests/zipfiles/manifest-name-override.zip` & `plone.resource-3.0.0/plone/resource/tests/zipfiles/manifest-name-override.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip` & `plone.resource-3.0.0/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/plone/resource/tests/zipfiles/normal.zip` & `plone.resource-3.0.0/plone/resource/tests/zipfiles/normal.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-2.1.4/plone/resource/traversal.py` & `plone.resource-3.0.0/plone/resource/traversal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
 from plone.resource.interfaces import IUniqueResourceRequest
 from plone.resource.utils import queryResourceDirectory
-from six.moves import urllib
 from zExceptions import NotFound
 from zope.interface import alsoProvides
 from zope.traversing.namespace import SimpleHandler
 
+import urllib
 
-class ResourceTraverser(SimpleHandler):
 
+class ResourceTraverser(SimpleHandler):
     name = None
 
     def __init__(self, context, request=None):
         self.context = context
 
     def traverse(self, name, remaining):
         _type = self.name
```

### Comparing `plone.resource-2.1.4/plone/resource/utils.py` & `plone.resource-3.0.0/plone/resource/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.resource.interfaces import IResourceDirectory
 from zExceptions import NotFound
 from zope.component import getUtilitiesFor
 from zope.component import queryUtility
 
 
 def iterDirectoriesOfType(type, filter_duplicates=True):
@@ -19,70 +18,76 @@
     - resource directories in distributions
     """
 
     found = set()
 
     # 1. Persistent resource directory:
     #    List (persistent resource directory)/$type
-    res = queryUtility(IResourceDirectory, name=u'persistent')
+    res = queryUtility(IResourceDirectory, name="persistent")
     if res and res.isDirectory(type):
         typedir = res[type]
         for dirname in typedir.listDirectory():
             if not typedir.isDirectory(dirname):
                 continue
             yield typedir[dirname]
             found.add(dirname)
 
     # 2. Global resource directory:
     #    List (global resource directory)/$type
-    res = queryUtility(IResourceDirectory, name=u'')
+    res = queryUtility(IResourceDirectory, name="")
     if res and res.isDirectory(type):
         typedir = res[type]
         for dirname in typedir.listDirectory():
             if not typedir.isDirectory(dirname):
                 continue
             if not filter_duplicates or dirname not in found:
                 yield typedir[dirname]
                 found.add(dirname)
 
     # 3. Packaged resource directories:
     #    Scan the registry
-    identifier = '++%s++' % type
+    identifier = "++%s++" % type
     for name, u in getUtilitiesFor(IResourceDirectory):
         if name.startswith(identifier):
             if not filter_duplicates or u.__name__ not in found:
                 yield u
 
 
 def queryResourceDirectory(type, name):
     """Find the IResourceDirectory of the given name and type. Returns
     None if not found.
     """
 
     # 1. Persistent resource directory:
     #    Try (persistent resource directory)/$type/$name
-    res = queryUtility(IResourceDirectory, name=u'persistent')
+    res = queryUtility(IResourceDirectory, name="persistent")
     if res:
         try:
             return res[type][name]
-        except (KeyError, NotFound,):
+        except (
+            KeyError,
+            NotFound,
+        ):
             pass  # pragma: no cover
 
     # 2. Global resource directory:
     #    Try (global resource directory)/$type/$name
-    res = queryUtility(IResourceDirectory, name=u'')
+    res = queryUtility(IResourceDirectory, name="")
     if res:
         try:
             return res[type][name]
-        except (KeyError, NotFound,):
+        except (
+            KeyError,
+            NotFound,
+        ):
             pass  # pragma: no cover
 
     # 3. Packaged type-specific resource directory:
     #    Try (directory named after type + name)
-    identifier = u'++%s++%s' % (type, name)
+    identifier = f"++{type}++{name}"
     res = queryUtility(IResourceDirectory, name=identifier)
     if res is not None:
         return res
 
     return None
 
 
@@ -97,8 +102,7 @@
             cloneResourceDirectory(source[name], target[name])
         else:
             f = source.openFile(name)
             try:
                 target.writeFile(name, f)
             finally:
                 f.close()
-
```

### Comparing `plone.resource-2.1.4/plone/resource/zcml.py` & `plone.resource-3.0.0/plone/resource/zcml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,84 @@
-# -*- coding: utf-8 -*-
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.interfaces import IResourceDirectory
 from zope.component.zcml import handler
 from zope.configuration.exceptions import ConfigurationError
 from zope.interface import Interface
-from zope.schema import ASCIILine, TextLine
+from zope.schema import ASCIILine
+from zope.schema import TextLine
 
 import os.path
 
 
 class IResourceDirectoryDirective(Interface):
-    """Register resource directories with the global registry.
-    """
+    """Register resource directories with the global registry."""
 
     directory = TextLine(
-        title=u'Directory path',
-        description=u'Path relative to the package.',
-        required=True
-        )
+        title="Directory path",
+        description="Path relative to the package.",
+        required=True,
+    )
 
     name = TextLine(
-        title=u'Name',
-        description=u'Name of the directory. If not specified, the name of '
-                    u'the current package is used.',
+        title="Name",
+        description="Name of the directory. If not specified, the name of "
+        "the current package is used.",
         required=False,
-        )
+    )
 
     type = ASCIILine(
-        title=u'Resource type',
+        title="Resource type",
         # XXX use a Choice field + vocab
         # vocabulary = 'plone.resource.vocab.ResourceTypes',
         required=False,
-        )
+    )
 
 
 def registerResourceDirectory(_context, directory, name=None, type=None):
     """
     Register a new resource directory.
 
     The actual ZCA registrations are deferred so that conflicts can be resolved
     via zope.configuration's discriminator machinery.
     """
 
     if _context.package and os.path.isabs(directory):
-        raise ConfigurationError('Resource directories in distributions must '
-                                 'be specified as relative paths.')
+        raise ConfigurationError(
+            "Resource directories in distributions must "
+            "be specified as relative paths."
+        )
     elif _context.package:
         directory = _context.path(directory)
     elif not _context.package and not os.path.isabs(directory):
-        raise ConfigurationError('Global resource directories must be '
-                                 'specified as absolute paths.')
+        raise ConfigurationError(
+            "Global resource directories must be " "specified as absolute paths."
+        )
 
     # TODO: make sure this works in Windows
-    if '..' in directory.split('/'):
-        raise ConfigurationError('Traversing to parent directories '
-                                 'via .. is not allowed.')
+    if ".." in directory.split("/"):
+        raise ConfigurationError(
+            "Traversing to parent directories " "via .. is not allowed."
+        )
     if not os.path.exists(directory):
-        raise IOError('Directory not found: %s' % directory)
+        raise OSError("Directory not found: %s" % directory)
 
     if name is None and _context.package:
         name = _context.package.__name__
 
     if type:
-        identifier = '++%s++%s' % (type, name or '')
+        identifier = "++{}++{}".format(type, name or "")
     else:
         if _context.package:
-            raise ConfigurationError('Resource directories in distributions '
-                                     'must have a specified resource type.')
-        identifier = name or ''
+            raise ConfigurationError(
+                "Resource directories in distributions "
+                "must have a specified resource type."
+            )
+        identifier = name or ""
 
-    directory = os.path.sep.join(directory.split('/'))
+    directory = os.path.sep.join(directory.split("/"))
     directory = FilesystemResourceDirectory(directory, name)
 
     _context.action(
-        discriminator=('plone:static', identifier),
+        discriminator=("plone:static", identifier),
         callable=handler,
-        args=('registerUtility', directory, IResourceDirectory, identifier),
-        )
+        args=("registerUtility", directory, IResourceDirectory, identifier),
+    )
```

### Comparing `plone.resource-2.1.4/plone.resource.egg-info/SOURCES.txt` & `plone.resource-3.0.0/plone.resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

