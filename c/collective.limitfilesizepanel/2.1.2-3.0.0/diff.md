# Comparing `tmp/collective.limitfilesizepanel-2.1.2.tar.gz` & `tmp/collective.limitfilesizepanel-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.limitfilesizepanel-2.1.2.tar", last modified: Tue Jul 17 10:59:22 2018, max compression
+gzip compressed data, was "collective.limitfilesizepanel-3.0.0.tar", last modified: Thu Apr 27 08:23:18 2023, max compression
```

## Comparing `collective.limitfilesizepanel-2.1.2.tar` & `collective.limitfilesizepanel-3.0.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/
--rw-r--r--   0 cekk       (503) staff       (20)     1210 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/buildout.cfg
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/
--rw-r--r--   0 cekk       (503) staff       (20)      192 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/__init__.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/
--rw-r--r--   0 cekk       (503) staff       (20)      221 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/__init__.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/
--rw-r--r--   0 cekk       (503) staff       (20)       24 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/__init__.py
--rw-r--r--   0 cekk       (503) staff       (20)     1321 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/configure.zcml
--rw-r--r--   0 cekk       (503) staff       (20)     2072 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/controlpanel.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/images/
--rw-r--r--   0 cekk       (503) staff       (20)      879 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
--rw-r--r--   0 cekk       (503) staff       (20)     9392 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
--rw-r--r--   0 cekk       (503) staff       (20)     1487 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/tinymce_upload_p5.py
--rw-r--r--   0 cekk       (503) staff       (20)     3041 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/configure.zcml
--rw-r--r--   0 cekk       (503) staff       (20)     1927 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/dx_validators.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/Extensions/
--rw-r--r--   0 cekk       (503) staff       (20)      441 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/Extensions/install.py
--rw-r--r--   0 cekk       (503) staff       (20)     3167 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/interfaces.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/
--rw-r--r--   0 cekk       (503) staff       (20)      620 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot
--rw-r--r--   0 cekk       (503) staff       (20)     2862 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/de/
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/
--rw-r--r--   0 cekk       (503) staff       (20)     1671 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo
--rw-r--r--   0 cekk       (503) staff       (20)     3494 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/it/
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (503) staff       (20)     2765 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo
--rw-r--r--   0 cekk       (503) staff       (20)     4044 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po
--rwxr-xr-x   0 cekk       (503) staff       (20)      240 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/rebuildPo.sh
--rw-r--r--   0 cekk       (503) staff       (20)     1214 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/overrides.zcml
--rw-r--r--   0 cekk       (503) staff       (20)     1401 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/patches.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/
--rw-r--r--   0 cekk       (503) staff       (20)      159 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (503) staff       (20)      733 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (503) staff       (20)      172 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (503) staff       (20)      112 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/registry.xml
--rw-r--r--   0 cekk       (503) staff       (20)      406 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/uninstall/
--rw-r--r--   0 cekk       (503) staff       (20)      183 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (503) staff       (20)      464 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (503) staff       (20)      561 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (503) staff       (20)      855 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/setuphandlers.py
--rw-r--r--   0 cekk       (503) staff       (20)     1411 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/testing.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/
--rw-r--r--   0 cekk       (503) staff       (20)       24 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/__init__.py
--rw-r--r--   0 cekk       (503) staff       (20)     1733 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/base.py
--rw-r--r--   0 cekk       (503) staff       (20)      598 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/base_dx.py
--rw-r--r--   0 cekk       (503) staff       (20)     1450 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_bypassvalidation.py
--rw-r--r--   0 cekk       (503) staff       (20)     5221 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_maxsizecalc.py
--rw-r--r--   0 cekk       (503) staff       (20)     3429 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
--rw-r--r--   0 cekk       (503) staff       (20)     1929 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_setup.py
--rw-r--r--   0 cekk       (503) staff       (20)     6154 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tinymce_upload_p4.py
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/
--rw-r--r--   0 cekk       (503) staff       (20)        1 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (503) staff       (20)       90 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (503) staff       (20)       11 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (503) staff       (20)        1 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (503) staff       (20)     7085 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (503) staff       (20)      198 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/requires.txt
--rw-r--r--   0 cekk       (503) staff       (20)     2911 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (503) staff       (20)       11 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/top_level.txt
-drwxr-xr-x   0 cekk       (503) staff       (20)        0 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/docs/
--rw-r--r--   0 cekk       (503) staff       (20)    30244 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/docs/collective.limitfilesizepanel-1.3-01.png
--rw-r--r--   0 cekk       (503) staff       (20)    21991 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/docs/collective.limitfilesizepanel-1.3-02.png
--rw-r--r--   0 cekk       (503) staff       (20)     1977 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/docs/HISTORY.rst
--rw-r--r--   0 cekk       (503) staff       (20)     1594 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/docs/INSTALL.txt
--rw-r--r--   0 cekk       (503) staff       (20)    17987 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/docs/LICENSE.GPL
--rw-r--r--   0 cekk       (503) staff       (20)      746 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/docs/LICENSE.txt
--rw-r--r--   0 cekk       (503) staff       (20)      214 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/MANIFEST.in
--rw-r--r--   0 cekk       (503) staff       (20)     7085 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/PKG-INFO
--rw-r--r--   0 cekk       (503) staff       (20)     2919 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/README.rst
--rw-r--r--   0 cekk       (503) staff       (20)       31 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/requirements.txt
--rw-r--r--   0 cekk       (503) staff       (20)       38 2018-07-17 10:59:22.000000 collective.limitfilesizepanel-2.1.2/setup.cfg
--rw-r--r--   0 cekk       (503) staff       (20)     1645 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/setup.py
--rw-r--r--   0 cekk       (503) staff       (20)     1089 2018-07-17 10:59:21.000000 collective.limitfilesizepanel-2.1.2/versions.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.970950 collective.limitfilesizepanel-3.0.0/
+-rw-r--r--   0 cekk       (501) staff       (20)      214 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     8211 2023-04-27 08:23:18.971144 collective.limitfilesizepanel-3.0.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3425 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     2059 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/base.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)       96 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/buildout.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.955978 collective.limitfilesizepanel-3.0.0/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)      193 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.960694 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.960974 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/Extensions/
+-rw-r--r--   0 cekk       (501) staff       (20)      450 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/Extensions/install.py
+-rw-r--r--   0 cekk       (501) staff       (20)      221 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.962449 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1321 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1457 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.962731 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/images/
+-rw-r--r--   0 cekk       (501) staff       (20)      879 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
+-rw-r--r--   0 cekk       (501) staff       (20)     5492 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1468 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/tinymce_upload_p5.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1827 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2760 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/dx_validators.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2458 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.963589 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      620 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     2862 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.951820 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.964158 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1671 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     3494 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.952096 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.964734 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2765 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     4044 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po
+-rwxr-xr-x   0 cekk       (501) staff       (20)      240 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/rebuildPo.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.952633 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.966314 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      159 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      733 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      112 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      406 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.967201 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      464 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      561 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2096 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1282 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.968922 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      592 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/base_dx.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1446 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_bypassvalidation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2631 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2534 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5054 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_validation.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1698 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.958396 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     8211 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2836 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       90 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      235 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-27 08:23:18.970668 collective.limitfilesizepanel-3.0.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     2205 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/HISTORY.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1594 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/INSTALL.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      746 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/LICENSE.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    30244 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-01.png
+-rw-r--r--   0 cekk       (501) staff       (20)    21991 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-02.png
+-rw-r--r--   0 cekk       (501) staff       (20)       42 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      346 2023-04-27 08:23:18.971693 collective.limitfilesizepanel-3.0.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1853 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1838 2023-04-27 08:23:18.000000 collective.limitfilesizepanel-3.0.0/test_plone52.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/configure.zcml` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/controlpanel.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/controlpanel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 # -*- coding: utf-8 -*-
-
-from Products.statusmessages.interfaces import IStatusMessage
 from collective.limitfilesizepanel import messageFactory as _
 from collective.limitfilesizepanel.interfaces import ILimitFileSizePanel
+from collective.limitfilesizepanel.interfaces import ITypesSettingsRow
+from collective.z3cform.jsonwidget.browser.widget import JSONFieldWidget
 from plone.app.registry.browser import controlpanel
-from z3c.form import button
+from Products.CMFPlone.resources import add_bundle_on_request
+from z3c.form import field
 
 
 class LimitFileSizeEditForm(controlpanel.RegistryEditForm):
-    """Media settings form.
-    """
+    """Media settings form."""
+
     schema = ILimitFileSizePanel
     id = "LimitFileSizeEditForm"
-    label = _(u"Limit file size settings")
-    description = _(u"help_limit_file_size_panel",
-                    default=u"Set file size for file and image")
-
-    @button.buttonAndHandler(_('Save'), name='save')
-    def handleSave(self, action):
-        data, errors = self.extractData()
-        if errors:
-            self.status = self.formErrorsMessage
-            return
-        self.applyChanges(data)
-        IStatusMessage(self.request).addStatusMessage(_(u"Changes saved"),
-                                                      "info")
-        self.context.REQUEST.RESPONSE.redirect("@@limitfilesize-settings")
-
-    @button.buttonAndHandler(_('Cancel'), name='cancel')
-    def handleCancel(self, action):
-        IStatusMessage(self.request).addStatusMessage(_(u"Edit cancelled"),
-                                                      "info")
-        self.request.response.redirect("%s/%s" % (self.context.absolute_url(),
-                                                  self.control_panel_view))
+    label = _("Limit file size settings")
+    description = _(
+        "help_limit_file_size_panel", default="Set file size for file and image"
+    )
+    fields = field.Fields(ILimitFileSizePanel)
+    fields["types_settings"].widgetFactory = JSONFieldWidget
 
     def updateWidgets(self):
-        super(LimitFileSizeEditForm, self).updateWidgets()
-        self.widgets['file_size'].maxlength = 5
-        self.widgets['file_size'].size = 5
-        self.widgets['image_size'].maxlength = 5
-        self.widgets['image_size'].size = 5
-        for widget in self.widgets['types_settings'].widgets:
-            widget.subform.widgets['size'].maxlength = 5
-            widget.subform.widgets['size'].size = 5
+        super().updateWidgets()
+        self.widgets["file_size"].maxlength = 5
+        self.widgets["file_size"].size = 5
+        self.widgets["image_size"].maxlength = 5
+        self.widgets["image_size"].size = 5
+        self.widgets["types_settings"].schema = ITypesSettingsRow
 
 
 class LimitFileSizeControlPanel(controlpanel.ControlPanelFormWrapper):
-    """Analytics settings control panel.
-    """
+    """Analytics settings control panel."""
+
+    def __call__(self):
+        add_bundle_on_request(self.request, "z3cform-jsonwidget-bundle")
+        return super().__call__()
+
     form = LimitFileSizeEditForm
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/images/limitfilesize-settings.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/browser/tinymce_upload_p5.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/browser/tinymce_upload_p5.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,35 @@
 
 class FileUpload(BaseFileUploadView):
     """
     add filesize validation to tinymce file upload view
     """
 
     def __call__(self):
-        filedata = self.request.form.get('file', None)
+        filedata = self.request.form.get("file", None)
         if not filedata:
             return super(FileUpload, self).__call__()
         filename = filedata.filename
-        content_type = mimetypes.guess_type(filename)[0] or ''
-        ctr = api.portal.get_tool(name='content_type_registry')
-        portal_type = ctr.findTypeName(
-            filename.lower(), content_type, '') or 'File'
+        content_type = mimetypes.guess_type(filename)[0] or ""
+        ctr = api.portal.get_tool(name="content_type_registry")
+        portal_type = ctr.findTypeName(filename.lower(), content_type, "") or "File"
 
         helper_view = api.content.get_view(
-            name='lfsp_helpers_view',
+            name="lfsp_helpers_view",
             context=self.context,
-            request=self.context.REQUEST,)
+            request=self.context.REQUEST,
+        )
 
-        if helper_view.newDataOnly() and '/edit' in self.request.get('HTTP_REFERER'):  # noqa
+        if helper_view.newDataOnly() and "/edit" in self.request.get(
+            "HTTP_REFERER"
+        ):  # noqa
             return super(FileUpload, self).__call__()
         maxsize = helper_view.get_maxsize_tiny((portal_type,))
         if not maxsize:
             return super(FileUpload, self).__call__()
 
-        size_check = helper_view.check_size_dx(
-            maxsize=maxsize,
-            uploadfile=filedata
-        )
-        if size_check and not size_check.get('valid', False):
+        size_check = helper_view.check_size(maxsize=maxsize, uploadfile=filedata)
+        if size_check and not size_check.get("valid", False):
             response = self.request.RESPONSE
             response.setStatus(403)
-            return size_check.get('error', '')
+            return size_check.get("error", "")
         return super(FileUpload, self).__call__()
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/configure.zcml` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/configure.zcml`

 * *Files 23% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 	  xmlns:monkey="http://namespaces.plone.org/monkey"
     i18n_domain="collective.limitfilesizepanel">
 
   <five:registerPackage package="." />
 
   <include package="plone.app.registry" />
   <include package="collective.monkeypatcher" />
-
+  
   <i18n:registerTranslations directory="locales" />
 
   <permission
         id="collective.limitfilesizepanel.LimitFileSizePanel"
         title="collective.limitfilesizepanel: Manage limit file size settings"
         />
   <permission
         id="collective.limitfilesizepanel.BypassLimitSize"
         title="collective.limitfilesizepanel: Bypass limit size"
         />
 
   <include package=".browser" />
-  <includeOverrides file="overrides.zcml" />
+  <include file="upgrades.zcml" />
 
   <genericsetup:registerProfile
       name="default"
       title="Limit files and images size"
       directory="profiles/default"
       description="Configure the file size limit from control panel"
       provides="Products.GenericSetup.interfaces.EXTENSION"
@@ -36,51 +36,16 @@
   <genericsetup:registerProfile
       name="uninstall"
       title="Remove collective.limitfilesizepanel"
       directory="profiles/uninstall"
       description=""
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
-  <genericsetup:upgradeStep
-        title="Upgrade to collective.limitfilesizepanel to version 1.1"
-        description="Migrates collective.limitfilesizepanel to 1000"
-        source="1.0"
-        destination="1000"
-        handler=".setuphandlers.migrateTo1000"
-        sortkey="1"
-        profile="collective.limitfilesizepanel:default"
-    />
-  <genericsetup:upgradeStep
-        title="Upgrade to collective.limitfilesizepanel to version 1.3"
-        description="Migrates collective.limitfilesizepanel to 1100"
-        source="11000"
-        destination="1100"
-        handler=".setuphandlers.migrateTo1100"
-        sortkey="2"
-        profile="collective.limitfilesizepanel:default"
-    />
-
-  <genericsetup:upgradeStep
-        title="Upgrade to collective.limitfilesizepanel to version 1200"
-        description="Migrates collective.limitfilesizepanel to 1200"
-        source="1100"
-        destination="1200"
-        handler=".setuphandlers.migrateTo1200"
-        sortkey="3"
-        profile="collective.limitfilesizepanel:default"
-    />
-
-  <monkey:patch
-     description="Patching MaxSizeValidator for apply the collective.limitfilesizepanel features"
-     class="Products.validation.validators.SupplValidators.MaxSizeValidator"
-     original="__call__"
-	   preserveOriginal="True"
-     replacement=".patches.patched__call__"
-     docstringWarning="true"
-    />
-
-    <configure zcml:condition="installed plone.dexterity">
-      <adapter factory=".dx_validators.FileSizeValidator" />
-      <adapter factory=".dx_validators.ImageFileSizeValidator" />
-    </configure>
+
+    <!-- <adapter factory=".dx_validators.FileSizeValidator" />
+    <adapter factory=".dx_validators.ImageFileSizeValidator" /> -->
+    <adapter factory=".dx_validators.FileSizeValidator" name="collective.limitfilesizepanel.file_size_validator" />
+    <adapter factory=".dx_validators.ImageSizeValidator" name="collective.limitfilesizepanel.image_size_validator" />
+
+
 
 </configure>
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/interfaces.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/interfaces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,89 @@
 # -*- coding: utf-8 -*-
-
 from collective.limitfilesizepanel import messageFactory as _
-from plone.registry.field import PersistentField
-from z3c.form.object import registerFactoryAdapter
 from zope import schema
 from zope.interface import Interface
-from zope.interface import implements
 
 
 class ILimitFileSizePanelLayer(Interface):
     """
     Browserlayer
     """
 
 
 class ICheckSizeUtility(Interface):
     """
     Marker interface for CheckSize utility
     """
 
 
-class ITypesSettings(Interface):
+class ITypesSettingsRow(Interface):
     """A single unit of size limit for a type and field name"""
 
     content_type = schema.Choice(
-        title=_(u"Content type"),
-        vocabulary='plone.app.vocabularies.ReallyUserFriendlyTypes',
-        required=True)
+        title=_("Content type"),
+        vocabulary="plone.app.vocabularies.ReallyUserFriendlyTypes",
+        required=True,
+    )
 
     field_name = schema.TextLine(
-        title=_(u"Field name"),
+        title=_("Field name"),
         description=_(
-            'help_field_name',
-            default=u"Low level field name, commonly \"image\" or \"file\"."),
-        required=True)
+            "help_field_name",
+            default='Low level field name, commonly "image" or "file".',
+        ),
+        required=True,
+    )
 
     size = schema.Int(
-        title=_(u"Size limit"),
+        title=_("Size limit"),
         description=_(
-            u"Type here a number in MB which will"
-            u" limit the field size upload"),
+            "Type here a number in MB which will" " limit the field size upload"
+        ),
         default=30,
-        required=True
+        required=True,
     )
 
 
-class TypesSettings(object):
-    implements(ITypesSettings)
-
-    def __init__(self, content_type=None, field_name=None, size=None):
-        self.content_type = content_type
-        self.field_name = field_name
-        self.size = size
-
-
-class PersistentObject(PersistentField, schema.Object):
-    pass
-
-
 class ILimitFileSizePanel(Interface):
     """
     Settings used in the control panel
     """
 
     file_size = schema.Int(
-        title=_(u"Set the file-type size limit"),
-        description=_(
-            u"Type here a number in MB which will limit the file size upload"),
+        title=_("Set the file-type size limit"),
+        description=_("Type here a number in MB which will limit the file size upload"),
         default=30,
     )
 
     image_size = schema.Int(
-        title=_(u"Set the image-type size limit"),
+        title=_("Set the image-type size limit"),
         description=_(
-            u"Type here a number in MB which will"
-            u" limit the image size upload"),
+            "Type here a number in MB which will" " limit the image size upload"
+        ),
         default=10,
     )
 
-    types_settings = schema.Tuple(
-        title=_(u'Settings for other content types and fields'),
+    types_settings = schema.SourceText(
+        title=_("Settings for other content types and fields"),
         description=_(
-            'help_types_settings',
-            default=u"Use this section to provide size overrides of"
-                    u" values above.\nProvide a content type/field ID,"
-                    u" and the size limit."),
-        value_type=PersistentObject(
-            ITypesSettings,
-            title=_(u"Content/field settings")),
+            "help_types_settings",
+            default="Use this section to provide size overrides of"
+            " values above.\nProvide a content type/field ID,"
+            " and the size limit.",
+        ),
         required=False,
-        default=(),
-        missing_value=(),
     )
 
     new_data_only = schema.Bool(
-        title=_(u"Validate only new data"),
+        title=_("Validate only new data"),
         description=_(
             "help_new_data_only",
-            default=u"Keep selected to validate only new uploaded files and"
-                    u" images.\nIf you unselect this and the size "
-                    u"configurations above will be lowered, is possible that"
-                    u" users that edit contents wont be able to save the form "
-                    u"because the validator will check also data already"
-                    u" saved."),
+            default="Keep selected to validate only new uploaded files and"
+            " images.\nIf you unselect this and the size "
+            "configurations above will be lowered, is possible that"
+            " users that edit contents wont be able to save the form "
+            "because the validator will check also data already"
+            " saved.",
+        ),
         default=True,
     )
-
-
-registerFactoryAdapter(ITypesSettings, TypesSettings)
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel-manual.pot`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/collective.limitfilesizepanel.pot`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.mo`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/de/LC_MESSAGES/collective.limitfilesizepanel.po`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.mo`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/locales/it/LC_MESSAGES/collective.limitfilesizepanel.po`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/default/controlpanel.xml` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/profiles/uninstall/registry.xml` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/testing.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/testing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 # -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
-from plone.testing import z2
 
 import collective.limitfilesizepanel
+import collective.z3cform.jsonwidget
 
 
 class LimitFileSizePanelLayer(PloneSandboxLayer):
-
-    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE, )
+    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         self.loadZCML(package=collective.limitfilesizepanel)
+        self.loadZCML(package=collective.z3cform.jsonwidget)
 
     def setUpPloneSite(self, portal):
-        applyProfile(portal, 'collective.limitfilesizepanel:default')
+        applyProfile(portal, "collective.limitfilesizepanel:default")
 
 
 LIMITFILESIZEPANEL_FIXTURE = LimitFileSizePanelLayer()
 
 
 LIMITFILESIZEPANEL_INTEGRATION_TESTING = IntegrationTesting(
     bases=(LIMITFILESIZEPANEL_FIXTURE,),
-    name='LimitFileSizePanelLayer:IntegrationTesting'
+    name="LimitFileSizePanelLayer:IntegrationTesting",
 )
 
 
 LIMITFILESIZEPANEL_FUNCTIONAL_TESTING = FunctionalTesting(
     bases=(LIMITFILESIZEPANEL_FIXTURE,),
-    name='LimitFileSizePanelLayer:FunctionalTesting'
-)
-
-
-LIMITFILESIZEPANEL_ACCEPTANCE_TESTING = FunctionalTesting(
-    bases=(
-        LIMITFILESIZEPANEL_FIXTURE,
-        z2.ZSERVER_FIXTURE
-    ),
-    name='LimitFileSizePanelLayer:AcceptanceTesting'
+    name="LimitFileSizePanelLayer:FunctionalTesting",
 )
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/base_dx.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/base_dx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # -*- coding: utf-8 -*-
 from plone.namedfile.field import NamedBlobFile, NamedBlobImage
 from zope import interface
 
 
 class ITestSchema(interface.Interface):
-
     file = NamedBlobFile(
-        title=u"Example file",
+        title="Example file",
         required=False,
     )
 
     image = NamedBlobImage(
-        title=u"Example image",
+        title="Example image",
         required=False,
     )
 
 
 class FileObject(object):
-
-    portal_type = 'File'  # we need a valid portal_type
+    portal_type = "File"  # we need a valid portal_type
 
 
 class NewsObject(object):
-
-    portal_type = 'News Item'  # we need a valid portal_type
+    portal_type = "News Item"  # we need a valid portal_type
 
 
 class ImageObject(object):
-
-    portal_type = 'Image'  # we need a valid portal_type
+    portal_type = "Image"  # we need a valid portal_type
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_bypassvalidation.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_bypassvalidation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # -*- coding: utf-8 -*-
-from collective.limitfilesizepanel.testing import LIMITFILESIZEPANEL_INTEGRATION_TESTING  # NOQA
+from collective.limitfilesizepanel.testing import (
+    LIMITFILESIZEPANEL_INTEGRATION_TESTING,
+)  # NOQA
 from plone import api
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import setRoles
 import unittest
 
 
 class TestBypassSize(unittest.TestCase):
     """
     This test cover the bypass size validation feature.
     """
 
     layer = LIMITFILESIZEPANEL_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Member'])
+        self.portal = self.layer["portal"]
+        setRoles(self.portal, TEST_USER_ID, ["Member"])
         self.helper_view = api.content.get_view(
-            name='lfsp_helpers_view',
+            name="lfsp_helpers_view",
             context=self.portal,
             request=self.portal.REQUEST,
         )
 
     def test_bypass_validation(self):
-        """
-        """
+        """ """
         # first check that current user can't bypass validation
         self.assertFalse(self.helper_view.canBypassValidation())
         # now set the permission to "Member" role
         self.portal.manage_permission(
-            'collective.limitfilesizepanel: Bypass limit size',
-            ['Member'],
-            acquire=False)
+            "collective.limitfilesizepanel: Bypass limit size",
+            ["Member"],
+            acquire=False,
+        )
         # now check that current user can bypass validation
         self.assertTrue(self.helper_view.canBypassValidation())
 
     def tearDown(self):
         """
         revert settings to default
         """
         self.portal.manage_permission(
-            'collective.limitfilesizepanel: Bypass limit size',
-            [],
-            acquire=False)
+            "collective.limitfilesizepanel: Bypass limit size", [], acquire=False
+        )
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,69 @@
 # -*- coding: utf-8 -*-
-from collective.limitfilesizepanel.dx_validators import DXFileSizeValidator
 from collective.limitfilesizepanel.interfaces import ILimitFileSizePanel
-from collective.limitfilesizepanel.interfaces import TypesSettings
-from collective.limitfilesizepanel.testing import LIMITFILESIZEPANEL_INTEGRATION_TESTING  # NOQA
-from collective.limitfilesizepanel.tests.base_dx import FileObject
-from collective.limitfilesizepanel.tests.base_dx import ImageObject
+from collective.limitfilesizepanel.testing import LIMITFILESIZEPANEL_INTEGRATION_TESTING
 from collective.limitfilesizepanel.tests.base_dx import ITestSchema
-from collective.limitfilesizepanel.tests.base_dx import NewsObject
 from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.registry.interfaces import IRegistry
 from zope.component import queryUtility
+
 import unittest
+import json
 
 
 class TestMaxSizeCalcDX(unittest.TestCase):
-
     layer = LIMITFILESIZEPANEL_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
-        self.installer = api.portal.get_tool('portal_quickinstaller')
+        self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
+
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+        self.installer = api.portal.get_tool("portal_quickinstaller")
         self.helper_view = api.content.get_view(
-            name='lfsp_helpers_view',
+            name="lfsp_helpers_view",
             context=self.portal,
-            request=self.portal.REQUEST,
+            request=self.request,
         )
         self.registry = queryUtility(IRegistry)
-        self.settings = self.registry.forInterface(ILimitFileSizePanel,
-                                                   check=False)
+        self.settings = self.registry.forInterface(ILimitFileSizePanel, check=False)
+
+    def tearDown(self):
+        self.settings.types_settings = ""
 
     def test_size_file_dx_from_registry(self):
         # original validator for file and image read maxsize from
         # zconf.ATFile.max_file_size at the end we have a number
         # so we pass maxsize=N.
         # By default in the registry we have 30MB for file and 10MB for images
         # and calling the validator with all the possible values, validation
         # should be done with user values
 
-        validator = DXFileSizeValidator(
-            None,
-            None,
-            FileObject(),
-            ITestSchema['file'],
-            None
-        )
-        self.assertEqual(float(30), self.helper_view.get_maxsize_dx(
-            validator,
-            ITestSchema['file'])
+        self.assertEqual(
+            float(30), self.helper_view.get_maxsize(field=ITestSchema["file"])
         )
 
     def test_size_image_dx_from_registry(self):
         # original validator for file and image read maxsize from
         # zconf.ATFile.max_file_size at the end we have a number
         # so we pass maxsize=N.
         # By default in the registry we have 30MB for file and 10MB for images
         # and calling the validator with all the possible values, validation
         # should be done with user values
 
-        validator = DXFileSizeValidator(
-            None,
-            None,
-            ImageObject(),
-            ITestSchema['image'],
-            None
-        )
-        self.assertEqual(float(10), self.helper_view.get_maxsize_dx(
-            validator,
-            ITestSchema['image'])
+        self.assertEqual(
+            float(10), self.helper_view.get_maxsize(field=ITestSchema["image"])
         )
 
-    def test_size_from_registry_type_setting_dx(self):
-        validator = DXFileSizeValidator(
-            None,
-            None,
-            NewsObject(),
-            ITestSchema['image'],
-            None
+    def test_size_from_registry_type_setting(self):
+        new_value = json.dumps(
+            [{"content_type": "News Item", "field_name": "image", "size": 7}]
         )
-        new_value = (TypesSettings(u'News Item', u'image', 7), )
-        self.settings.types_settings += new_value
+        self.settings.types_settings = new_value
         self.assertEqual(
             float(7),
-            self.helper_view.get_maxsize_dx(
-                validator,
-                ITestSchema['image'])
-            )
-        self.settings.types_settings = ()
+            self.helper_view.get_maxsize(
+                field=ITestSchema["image"], portal_type="News Item"
+            ),
+        )
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective/limitfilesizepanel/tests/test_setup.py` & `collective.limitfilesizepanel-3.0.0/collective/limitfilesizepanel/tests/test_setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
+from collective.limitfilesizepanel.testing import (
+    LIMITFILESIZEPANEL_INTEGRATION_TESTING,
+)  # noqa
 from plone import api
-from collective.limitfilesizepanel.testing import LIMITFILESIZEPANEL_INTEGRATION_TESTING  # noqa
+from plone.app.testing import setRoles
+from plone.app.testing import TEST_USER_ID
 
 import unittest
 
 
+try:
+    from Products.CMFPlone.utils import get_installer
+except ImportError:
+    get_installer = None
+
+
 class TestSetup(unittest.TestCase):
     """Test that collective.limitfilesizepanel is properly installed."""
 
     layer = LIMITFILESIZEPANEL_INTEGRATION_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
-        self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
+        self.portal = self.layer["portal"]
+        if get_installer:
+            self.installer = get_installer(self.portal, self.layer["request"])
+        else:
+            self.installer = api.portal.get_tool("portal_quickinstaller")
 
     def test_product_installed(self):
         """Test if collective.limitfilesizepanel is installed."""
-        self.assertTrue(self.installer.isProductInstalled(
-            'collective.limitfilesizepanel'))
+        self.assertTrue(
+            self.installer.isProductInstalled("collective.limitfilesizepanel")
+        )
 
     def test_browserlayer(self):
         """Test that ILimitFileSizePanelLayer is registered."""
-        from collective.limitfilesizepanel.interfaces import \
-            ILimitFileSizePanelLayer
+        from collective.limitfilesizepanel.interfaces import ILimitFileSizePanelLayer
         from plone.browserlayer import utils
+
         self.assertIn(ILimitFileSizePanelLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
-
     layer = LIMITFILESIZEPANEL_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
-        self.installer.uninstallProducts(['collective.limitfilesizepanel'])
+        self.portal = self.layer["portal"]
+        if get_installer:
+            self.installer = get_installer(self.portal, self.layer["request"])
+        else:
+            self.installer = api.portal.get_tool("portal_quickinstaller")
+        roles_before = api.user.get_roles(TEST_USER_ID)
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+        self.installer.uninstallProducts(["collective.limitfilesizepanel"])
+        setRoles(self.portal, TEST_USER_ID, roles_before)
 
     def test_product_uninstalled(self):
         """Test if collective.limitfilesizepanel is cleanly uninstalled."""
-        self.assertFalse(self.installer.isProductInstalled(
-            'collective.limitfilesizepanel'))
+        self.assertFalse(
+            self.installer.isProductInstalled("collective.limitfilesizepanel")
+        )
 
     def test_browserlayer_removed(self):
         """Test that ILimitFileSizePanelLayer is removed."""
-        from collective.limitfilesizepanel.interfaces import \
-            ILimitFileSizePanelLayer
+        from collective.limitfilesizepanel.interfaces import ILimitFileSizePanelLayer
         from plone.browserlayer import utils
+
         self.assertNotIn(ILimitFileSizePanelLayer, utils.registered_layers())
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/PKG-INFO` & `collective.limitfilesizepanel-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 Metadata-Version: 2.1
 Name: collective.limitfilesizepanel
-Version: 2.1.2
+Version: 3.0.0
 Summary: Configure files and images size limit through Plone control panel
 Home-page: http://plone.org/products/collective.limitfilesizepanel
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
-License: GPL
-Description: .. image:: https://travis-ci.org/RedTurtle/collective.limitfilesizepanel.svg?branch=master
-            :target: https://travis-ci.org/RedTurtle/collective.limitfilesizepanel
+License: GPL version 2
+Description: This is an helper package that setup a RedTurtle's Plone site ready to work with Volto.
         
-        Introduction
-        ============
         
-        Plone Archetypes framework already gives you a max size validation for files and images, but the default
-        configuration has some drawbacks:
+        |python| |version| |ci| |coverage| |downloads| |license|
+        
+        .. |python| image:: https://img.shields.io/pypi/pyversions/collective.limitfilesizepanel.svg
+          :target: https://pypi.python.org/pypi/collective.limitfilesizepanel/
+        
+        .. |version| image:: http://img.shields.io/pypi/v/collective.limitfilesizepanel.svg
+          :target: https://pypi.python.org/pypi/collective.limitfilesizepanel
+        
+        .. |ci| image:: https://github.com/RedTurtle/collective.limitfilesizepanel/actions/workflows/tests.yml/badge.svg
+          :target: https://github.com/RedTurtle/collective.limitfilesizepanel/actions
         
-        * is not simple to customize (best way is to use `plone.recipe.atcontenttypes`__)
-        * is the same for every Plone site of the environment
+        .. |downloads| image:: https://img.shields.io/pypi/dm/collective.limitfilesizepanel.svg
+           :target: https://pypi.org/project/collective.limitfilesizepanel/
         
-        __ http://pypi.python.org/pypi/plone.recipe.atcontenttypes/
+        .. |license| image:: https://img.shields.io/pypi/l/collective.limitfilesizepanel.svg
+            :target: https://pypi.org/project/collective.limitfilesizepanel/
+            :alt: License
         
-        This product will let you customize this validation from Plone user interface.
+        .. |coverage| image:: https://coveralls.io/repos/github/redturtle/collective.limitfilesizepanel/badge.svg?branch=master
+            :target: https://coveralls.io/github/redturtle/collective.limitfilesizepanel?branch=main
+            :alt: Coverage
+            
+        
+        Introduction
+        ============
+        
+        This product allows you to set a max siza validation for file and image fields in content-types.
         
         How to use it
         =============
         
         Just add the product to the buildout and install it in the site you want to use.
         
         A new "*Limit file size settings*" option will be added in the control panel, where you can change the
@@ -51,28 +66,22 @@
         ================
         
         If some users need to bypass the validation and upload some larger files, there is a new permission
         "*collective.limitfilesizepanel: Bypass limit size*" that allows to do this.
         
         You only need to set this permission to some roles, and they'll have no upload limits.
         
-        Dependencies
-        ============
-        
-        This products has been tested on:
+        Compatibility
+        =============
         
-        * Plone 3.3
-        * Plone 4.2
-        * Plone 4.3
+        This products runs on Python3 and has been tested on:
         
-        It's based on `plone.app.registry`__ that it not part of Plone on 3.3 version. You need to be
-        sure that a compatible version is used (in my experience: use `version 1.0b1`__).
+        * Plone 5.2
         
-         __ http://pypi.python.org/pypi/plone.app.registry
-         __ http://pypi.python.org/pypi/plone.app.registry/1.0b1
+        For older versions, please refer to 2.x branch/tags
         
         Credits
         =======
         
         Developed with the support of:
         
         * `Regione Emilia Romagna`__
@@ -95,14 +104,25 @@
         .. image:: http://www.redturtle.it/redturtle_banner.png
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.it/
         
         Changelog
         =========
         
+        3.0.0 (2023-04-27)
+        ------------------
+        
+        - Python3 support.
+          [cekk]
+        - Drop usage of persistent fields in registry. Now we use collective.z3cform.jsonwidget.
+          [cekk]
+        - Change validator to work also with restapi calls.
+          [cekk]
+        
+        
         2.1.2 (2018-07-17)
         ------------------
         
         - Fix release
           [cekk]
         
         2.1.1 (2018-07-17)
@@ -200,14 +220,18 @@
         1.0 (Unreleased)
         ----------------
         
         - Initial release
         
 Keywords: plone plonegov limit filesize validation
 Platform: UNKNOWN
+Classifier: Environment :: Web Environment
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 3.3
-Classifier: Framework :: Plone :: 4.2
-Classifier: Framework :: Plone :: 4.3
-Classifier: Framework :: Plone :: 5.0
+Classifier: Framework :: Plone :: Addon
+Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Requires-Python: >=3.7
 Provides-Extra: test
```

### Comparing `collective.limitfilesizepanel-2.1.2/collective.limitfilesizepanel.egg-info/SOURCES.txt` & `collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 MANIFEST.in
 README.rst
+base.cfg
 buildout.cfg
+constraints.txt
+constraints_plone52.txt
 requirements.txt
+setup.cfg
 setup.py
-versions.cfg
+test_plone52.cfg
 collective/__init__.py
 collective.limitfilesizepanel.egg-info/PKG-INFO
 collective.limitfilesizepanel.egg-info/SOURCES.txt
 collective.limitfilesizepanel.egg-info/dependency_links.txt
 collective.limitfilesizepanel.egg-info/entry_points.txt
 collective.limitfilesizepanel.egg-info/namespace_packages.txt
 collective.limitfilesizepanel.egg-info/not-zip-safe
 collective.limitfilesizepanel.egg-info/requires.txt
 collective.limitfilesizepanel.egg-info/top_level.txt
 collective/limitfilesizepanel/__init__.py
 collective/limitfilesizepanel/configure.zcml
 collective/limitfilesizepanel/dx_validators.py
 collective/limitfilesizepanel/interfaces.py
-collective/limitfilesizepanel/overrides.zcml
-collective/limitfilesizepanel/patches.py
 collective/limitfilesizepanel/setuphandlers.py
 collective/limitfilesizepanel/testing.py
-collective/limitfilesizepanel/tinymce_upload_p4.py
+collective/limitfilesizepanel/upgrades.zcml
 collective/limitfilesizepanel/Extensions/install.py
 collective/limitfilesizepanel/browser/__init__.py
 collective/limitfilesizepanel/browser/configure.zcml
 collective/limitfilesizepanel/browser/controlpanel.py
 collective/limitfilesizepanel/browser/limitfilesizepanel_view.py
 collective/limitfilesizepanel/browser/tinymce_upload_p5.py
 collective/limitfilesizepanel/browser/images/limitfilesize-settings.png
@@ -41,19 +43,18 @@
 collective/limitfilesizepanel/profiles/default/metadata.xml
 collective/limitfilesizepanel/profiles/default/registry.xml
 collective/limitfilesizepanel/profiles/default/rolemap.xml
 collective/limitfilesizepanel/profiles/uninstall/browserlayer.xml
 collective/limitfilesizepanel/profiles/uninstall/controlpanel.xml
 collective/limitfilesizepanel/profiles/uninstall/registry.xml
 collective/limitfilesizepanel/tests/__init__.py
-collective/limitfilesizepanel/tests/base.py
 collective/limitfilesizepanel/tests/base_dx.py
 collective/limitfilesizepanel/tests/test_bypassvalidation.py
-collective/limitfilesizepanel/tests/test_maxsizecalc.py
 collective/limitfilesizepanel/tests/test_maxsizecalc_dx.py
 collective/limitfilesizepanel/tests/test_setup.py
+collective/limitfilesizepanel/tests/test_validation.py
 docs/HISTORY.rst
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 docs/collective.limitfilesizepanel-1.3-01.png
 docs/collective.limitfilesizepanel-1.3-02.png
```

### Comparing `collective.limitfilesizepanel-2.1.2/docs/collective.limitfilesizepanel-1.3-01.png` & `collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-01.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/docs/collective.limitfilesizepanel-1.3-02.png` & `collective.limitfilesizepanel-3.0.0/docs/collective.limitfilesizepanel-1.3-02.png`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/docs/HISTORY.rst` & `collective.limitfilesizepanel-3.0.0/docs/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+3.0.0 (2023-04-27)
+------------------
+
+- Python3 support.
+  [cekk]
+- Drop usage of persistent fields in registry. Now we use collective.z3cform.jsonwidget.
+  [cekk]
+- Change validator to work also with restapi calls.
+  [cekk]
+
+
 2.1.2 (2018-07-17)
 ------------------
 
 - Fix release
   [cekk]
 
 2.1.1 (2018-07-17)
```

### Comparing `collective.limitfilesizepanel-2.1.2/docs/INSTALL.txt` & `collective.limitfilesizepanel-3.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/docs/LICENSE.GPL` & `collective.limitfilesizepanel-3.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/docs/LICENSE.txt` & `collective.limitfilesizepanel-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.limitfilesizepanel-2.1.2/PKG-INFO` & `collective.limitfilesizepanel-3.0.0/collective.limitfilesizepanel.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 Metadata-Version: 2.1
 Name: collective.limitfilesizepanel
-Version: 2.1.2
+Version: 3.0.0
 Summary: Configure files and images size limit through Plone control panel
 Home-page: http://plone.org/products/collective.limitfilesizepanel
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
-License: GPL
-Description: .. image:: https://travis-ci.org/RedTurtle/collective.limitfilesizepanel.svg?branch=master
-            :target: https://travis-ci.org/RedTurtle/collective.limitfilesizepanel
+License: GPL version 2
+Description: This is an helper package that setup a RedTurtle's Plone site ready to work with Volto.
         
-        Introduction
-        ============
         
-        Plone Archetypes framework already gives you a max size validation for files and images, but the default
-        configuration has some drawbacks:
+        |python| |version| |ci| |coverage| |downloads| |license|
+        
+        .. |python| image:: https://img.shields.io/pypi/pyversions/collective.limitfilesizepanel.svg
+          :target: https://pypi.python.org/pypi/collective.limitfilesizepanel/
+        
+        .. |version| image:: http://img.shields.io/pypi/v/collective.limitfilesizepanel.svg
+          :target: https://pypi.python.org/pypi/collective.limitfilesizepanel
+        
+        .. |ci| image:: https://github.com/RedTurtle/collective.limitfilesizepanel/actions/workflows/tests.yml/badge.svg
+          :target: https://github.com/RedTurtle/collective.limitfilesizepanel/actions
         
-        * is not simple to customize (best way is to use `plone.recipe.atcontenttypes`__)
-        * is the same for every Plone site of the environment
+        .. |downloads| image:: https://img.shields.io/pypi/dm/collective.limitfilesizepanel.svg
+           :target: https://pypi.org/project/collective.limitfilesizepanel/
         
-        __ http://pypi.python.org/pypi/plone.recipe.atcontenttypes/
+        .. |license| image:: https://img.shields.io/pypi/l/collective.limitfilesizepanel.svg
+            :target: https://pypi.org/project/collective.limitfilesizepanel/
+            :alt: License
         
-        This product will let you customize this validation from Plone user interface.
+        .. |coverage| image:: https://coveralls.io/repos/github/redturtle/collective.limitfilesizepanel/badge.svg?branch=master
+            :target: https://coveralls.io/github/redturtle/collective.limitfilesizepanel?branch=main
+            :alt: Coverage
+            
+        
+        Introduction
+        ============
+        
+        This product allows you to set a max siza validation for file and image fields in content-types.
         
         How to use it
         =============
         
         Just add the product to the buildout and install it in the site you want to use.
         
         A new "*Limit file size settings*" option will be added in the control panel, where you can change the
@@ -51,28 +66,22 @@
         ================
         
         If some users need to bypass the validation and upload some larger files, there is a new permission
         "*collective.limitfilesizepanel: Bypass limit size*" that allows to do this.
         
         You only need to set this permission to some roles, and they'll have no upload limits.
         
-        Dependencies
-        ============
-        
-        This products has been tested on:
+        Compatibility
+        =============
         
-        * Plone 3.3
-        * Plone 4.2
-        * Plone 4.3
+        This products runs on Python3 and has been tested on:
         
-        It's based on `plone.app.registry`__ that it not part of Plone on 3.3 version. You need to be
-        sure that a compatible version is used (in my experience: use `version 1.0b1`__).
+        * Plone 5.2
         
-         __ http://pypi.python.org/pypi/plone.app.registry
-         __ http://pypi.python.org/pypi/plone.app.registry/1.0b1
+        For older versions, please refer to 2.x branch/tags
         
         Credits
         =======
         
         Developed with the support of:
         
         * `Regione Emilia Romagna`__
@@ -95,14 +104,25 @@
         .. image:: http://www.redturtle.it/redturtle_banner.png
            :alt: RedTurtle Technology Site
            :target: http://www.redturtle.it/
         
         Changelog
         =========
         
+        3.0.0 (2023-04-27)
+        ------------------
+        
+        - Python3 support.
+          [cekk]
+        - Drop usage of persistent fields in registry. Now we use collective.z3cform.jsonwidget.
+          [cekk]
+        - Change validator to work also with restapi calls.
+          [cekk]
+        
+        
         2.1.2 (2018-07-17)
         ------------------
         
         - Fix release
           [cekk]
         
         2.1.1 (2018-07-17)
@@ -200,14 +220,18 @@
         1.0 (Unreleased)
         ----------------
         
         - Initial release
         
 Keywords: plone plonegov limit filesize validation
 Platform: UNKNOWN
+Classifier: Environment :: Web Environment
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 3.3
-Classifier: Framework :: Plone :: 4.2
-Classifier: Framework :: Plone :: 4.3
-Classifier: Framework :: Plone :: 5.0
+Classifier: Framework :: Plone :: Addon
+Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Requires-Python: >=3.7
 Provides-Extra: test
```

### Comparing `collective.limitfilesizepanel-2.1.2/setup.py` & `collective.limitfilesizepanel-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 from setuptools import setup, find_packages
 import os
 
-version = '2.1.2'
+version = "3.0.0"
 
 tests_require = [
-    'plone.app.testing',
-    'plone.testing>=5.0.0',
-    'plone.app.contenttypes',
-    'plone.app.robotframework[debug]',
-    ]
+    "plone.app.testing",
+    "plone.testing>=5.0.0",
+    "plone.app.contenttypes",
+    "plone.app.robotframework[debug]",
+]
 
-setup(name='collective.limitfilesizepanel',
-      version=version,
-      description="Configure files and images size limit through Plone control panel",
-      long_description=open("README.rst").read() + "\n" +
-                       open(os.path.join("docs", "HISTORY.rst")).read(),
-      # Get more strings from
-      # http://pypi.python.org/pypi?:action=list_classifiers
-      classifiers=[
+setup(
+    name="collective.limitfilesizepanel",
+    version=version,
+    description="Configure files and images size limit through Plone control panel",
+    long_description=open("README.rst").read()
+    + "\n"
+    + open(os.path.join("docs", "HISTORY.rst")).read(),
+    # Get more strings from
+    # http://pypi.python.org/pypi?:action=list_classifiers
+    classifiers=[
+        "Environment :: Web Environment",
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 3.3",
-        "Framework :: Plone :: 4.2",
-        "Framework :: Plone :: 4.3",
-        "Framework :: Plone :: 5.0",
+        "Framework :: Plone :: Addon",
+        "Framework :: Plone :: 5.2",
         "Programming Language :: Python",
-        ],
-      keywords='plone plonegov limit filesize validation',
-      author='RedTurtle Technology',
-      author_email='sviluppoplone@redturtle.it',
-      url='http://plone.org/products/collective.limitfilesizepanel',
-      license='GPL',
-      packages=find_packages(exclude=['ez_setup']),
-      namespace_packages=['collective'],
-      include_package_data=True,
-      zip_safe=False,
-      tests_require=tests_require,
-      extras_require=dict(test=tests_require),
-      install_requires=[
-          'setuptools',
-          'plone.api',
-          'plone.app.registry',
-          'collective.monkeypatcher>=1.0',
-          'plone.api',
-          'z3c.unconfigure'
-      ],
-      entry_points="""
+        "Programming Language :: Python :: 3.8",
+        "Operating System :: OS Independent",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+    ],
+    keywords="plone plonegov limit filesize validation",
+    author="RedTurtle Technology",
+    author_email="sviluppoplone@redturtle.it",
+    url="http://plone.org/products/collective.limitfilesizepanel",
+    license="GPL version 2",
+    python_requires=">=3.7",
+    packages=find_packages(exclude=["ez_setup"]),
+    namespace_packages=["collective"],
+    include_package_data=True,
+    zip_safe=False,
+    tests_require=tests_require,
+    extras_require=dict(test=tests_require),
+    install_requires=[
+        "setuptools",
+        "plone.api",
+        "plone.app.registry",
+        "collective.monkeypatcher>=1.0",
+        "plone.api",
+        "z3c.unconfigure",
+        "collective.z3cform.jsonwidget>=1.1.2",
+    ],
+    entry_points="""
       # -*- Entry points: -*-
 
       [z3c.autoinclude.plugin]
       target = plone
       """,
-      )
+)
```

