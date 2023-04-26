# Comparing `tmp/plone.theme-3.0.7.tar.gz` & `tmp/plone.theme-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.theme-3.0.7.tar", last modified: Wed Apr 22 21:25:54 2020, max compression
+gzip compressed data, was "plone.theme-4.0.0.tar", last modified: Wed Apr 26 22:07:17 2023, max compression
```

## Comparing `plone.theme-3.0.7.tar` & `plone.theme-4.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:25:54.000000 plone.theme-3.0.7/
--rw-r--r--   0 maurits    (501) staff       (20)     9214 2020-04-22 21:25:54.000000 plone.theme-3.0.7/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-22 21:25:53.000000 plone.theme-3.0.7/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-22 21:25:53.000000 plone.theme-3.0.7/pyproject.toml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9214 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      764 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)      121 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone.theme.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      149 2020-04-22 21:25:53.000000 plone.theme-3.0.7/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:25:54.000000 plone.theme-3.0.7/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2020-04-22 21:25:53.000000 plone.theme-3.0.7/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      673 2020-04-22 21:25:53.000000 plone.theme-3.0.7/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1906 2020-04-22 21:25:53.000000 plone.theme-3.0.7/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      244 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone/theme/
--rw-r--r--   0 maurits    (501) staff       (20)      187 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      296 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:25:54.000000 plone.theme-3.0.7/plone/theme/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       99 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/default.pt
--rw-r--r--   0 maurits    (501) staff       (20)      323 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      590 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/tests.zcml
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      100 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/mytheme.pt
--rw-r--r--   0 maurits    (501) staff       (20)      384 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/test_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)     4144 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/tests/testBrowserLayerPrecedence.py
--rw-r--r--   0 maurits    (501) staff       (20)        2 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1703 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)     3023 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      658 2020-04-22 21:25:53.000000 plone.theme-3.0.7/plone/theme/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)       67 2020-04-22 21:25:54.000000 plone.theme-3.0.7/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       69 2020-04-22 21:25:53.000000 plone.theme-3.0.7/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2883 2020-04-22 21:25:53.000000 plone.theme-3.0.7/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:07:17.273328 plone.theme-4.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     3071 2023-04-26 22:07:16.000000 plone.theme-4.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 22:07:16.000000 plone.theme-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 22:07:16.000000 plone.theme-4.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     7137 2023-04-26 22:07:17.273431 plone.theme-4.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)       69 2023-04-26 22:07:16.000000 plone.theme-4.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:07:17.267061 plone.theme-4.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 22:07:16.000000 plone.theme-4.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      673 2023-04-26 22:07:16.000000 plone.theme-4.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:07:17.267346 plone.theme-4.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:07:17.270858 plone.theme-4.0.0/plone/theme/
+-rw-r--r--   0 maurits    (501) staff       (20)     3047 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      182 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1803 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      628 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:07:17.272960 plone.theme-4.0.0/plone/theme/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/default.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      318 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      128 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/mytheme.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4058 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/testBrowserLayerPrecedence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      513 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/test_doctest.py
+-rw-r--r--   0 maurits    (501) staff       (20)      567 2023-04-26 22:07:16.000000 plone.theme-4.0.0/plone/theme/tests/tests.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:07:17.269307 plone.theme-4.0.0/plone.theme.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     7137 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      764 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:07:17.000000 plone.theme-4.0.0/plone.theme.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2858 2023-04-26 22:07:16.000000 plone.theme-4.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 22:07:17.273868 plone.theme-4.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1687 2023-04-26 22:07:16.000000 plone.theme-4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.theme-3.0.7/plone.theme.egg-info/SOURCES.txt` & `plone.theme-4.0.0/plone.theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.theme-3.0.7/docs/LICENSE.GPL` & `plone.theme-4.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.theme-3.0.7/docs/LICENSE.txt` & `plone.theme-4.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.theme-3.0.7/setup.py` & `plone.theme-4.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,64 @@
+from setuptools import find_packages
+from setuptools import setup
+
 import os
-from setuptools import setup, find_packages
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
-version = '3.0.7'
+
+version = "4.0.0"
 
 long_description = (
-    read('README.rst')
-    + '\n' +
-    read('plone', 'theme', 'README.rst')
-    + '\n' +
-    read('CHANGES.rst')
-    + '\n'
-    )
-
-
-setup(name='plone.theme',
-      version=version,
-      description="Tools for managing themes in CMF and Plone sites",
-      long_description=long_description,
-      classifiers=[
-          "Development Status :: 5 - Production/Stable",
-          "Environment :: Web Environment",
-          "Framework :: Plone",
-          "Framework :: Plone :: 5.0",
-          "Framework :: Plone :: 5.1",
-          "Framework :: Plone :: 5.2",
-          "Framework :: Plone :: Core",
-          "Framework :: Zope2",
-          "Framework :: Zope :: 4",
-          "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-          "Operating System :: OS Independent",
-          "Programming Language :: Python",
-          "Programming Language :: Python :: 2.7",
-          "Programming Language :: Python :: 3.6",
-          "Programming Language :: Python :: 3.7",
-          "Programming Language :: Python :: 3.8",
-      ],
-      keywords='plone theme manage',
-      author='Plone Foundation',
-      author_email='plone-developers@lists.sourceforge.net',
-      url='https://pypi.org/project/plone.theme',
-      license='GPL version 2',
-      packages=find_packages(),
-      namespace_packages=['plone'],
-      include_package_data=True,
-      zip_safe=False,
-      extras_require=dict(
-          test=[
-              'plone.app.testing',
-          ]
-      ),
-      install_requires=[
-          'setuptools',
-          'zope.component',
-          'zope.interface',
-          'zope.publisher',
-          'zope.traversing',
-          'Products.CMFCore',
-          'Zope2',
-      ],
-      )
+    read("README.rst")
+    + "\n"
+    + read("plone", "theme", "README.rst")
+    + "\n"
+    + read("CHANGES.rst")
+    + "\n"
+)
+
+
+setup(
+    name="plone.theme",
+    version=version,
+    description="Tools for managing themes in CMF and Plone sites",
+    long_description=long_description,
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Plone",
+        "Framework :: Plone :: 6.0",
+        "Framework :: Plone :: Core",
+        "Framework :: Zope :: 5",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    keywords="plone theme manage",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/plone.theme",
+    license="GPL version 2",
+    packages=find_packages(),
+    namespace_packages=["plone"],
+    include_package_data=True,
+    zip_safe=False,
+    python_requires=">=3.8",
+    extras_require=dict(
+        test=[
+            "plone.app.testing",
+            "plone.testing",
+        ]
+    ),
+    install_requires=[
+        "setuptools",
+        "Products.CMFCore",
+        "Zope",
+    ],
+)
```

### Comparing `plone.theme-3.0.7/plone/theme/tests/tests.zcml` & `plone.theme-4.0.0/plone/theme/tests/tests.zcml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser">
+    xmlns:browser="http://namespaces.zope.org/browser"
+    >
 
-    <interface
+  <interface
       interface=".interfaces.IMyTheme"
       type="zope.publisher.interfaces.browser.IBrowserSkinType"
       name="My Theme"
       />
 
-    <browser:page
-        name="layer-test-view"
-        for="*"
-        template="default.pt"
-        permission="zope2.View"
-        />
+  <browser:page
+      name="layer-test-view"
+      for="*"
+      template="default.pt"
+      permission="zope2.View"
+      />
 
-    <browser:page
-        name="layer-test-view"
-        for="*"
-        layer=".interfaces.IMyTheme"
-        template="mytheme.pt"
-        permission="zope2.View"
-        />
+  <browser:page
+      name="layer-test-view"
+      for="*"
+      template="mytheme.pt"
+      permission="zope2.View"
+      layer=".interfaces.IMyTheme"
+      />
 
 </configure>
```

### Comparing `plone.theme-3.0.7/plone/theme/tests/testBrowserLayerPrecedence.py` & `plone.theme-4.0.0/plone/theme/tests/testBrowserLayerPrecedence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This test confirms that views assigned to theme-specific layers
 # take precedence over views assigned to other kinds of layers.
 
 from plone.theme.interfaces import IDefaultPloneLayer
 from plone.theme.testing import PLONETHEME_INTEGRATION_TESTING
-
-from zope.event import notify
-from zope.interface import Interface, directlyProvides, directlyProvidedBy
 from zope.component import getGlobalSiteManager
+from zope.event import notify
+from zope.interface import directlyProvidedBy
+from zope.interface import directlyProvides
+from zope.interface import Interface
+from zope.publisher.browser import setDefaultSkin
 from zope.publisher.interfaces.browser import IBrowserSkinType
 from zope.publisher.interfaces.browser import IDefaultBrowserLayer
-from zope.publisher.browser import setDefaultSkin
 from zope.traversing.interfaces import BeforeTraverseEvent
 
 import unittest
 
 
 class IThemeSpecific(IDefaultPloneLayer):
     pass
@@ -24,33 +25,31 @@
 
 
 class IAdditiveLayerExtendingDefault(IDefaultPloneLayer):
     pass
 
 
 class LayerPrecedenceTestCase(unittest.TestCase):
-
     layer = PLONETHEME_INTEGRATION_TESTING
 
     additive_layer = None
     theme_layer = None
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
         gsm = getGlobalSiteManager()
         if self.theme_layer is not None:
             self._skin_name = self.portal.portal_skins.getDefaultSkin()
-            self._old_theme_layer = gsm.queryUtility(IBrowserSkinType,
-                                                     name=self._skin_name)
-            gsm.registerUtility(self.theme_layer,
-                                IBrowserSkinType,
-                                self._skin_name)
+            self._old_theme_layer = gsm.queryUtility(
+                IBrowserSkinType, name=self._skin_name
+            )
+            gsm.registerUtility(self.theme_layer, IBrowserSkinType, self._skin_name)
 
     def _get_request_interfaces(self):
-        request = self.layer['request']
+        request = self.layer["request"]
         setDefaultSkin(request)
         orig_iro = list(directlyProvidedBy(request).__iro__)
         directlyProvides(request, [self.additive_layer] + orig_iro)
         # Reset markers so that we can still register new skins and browserlayers
         del request._plonebrowserlayer_
         del request._plonetheme_
         notify(BeforeTraverseEvent(self.portal, request))
@@ -74,21 +73,20 @@
             # unless there are theme layers which extend them.
             self.assertTrue(additive_layer_pos < plone_default_pos)
         self.assertTrue(additive_layer_pos < zope_default_pos)
 
     def beforeTearDown(self):
         gsm = getGlobalSiteManager()
         if self.theme_layer is not None:
-            res = gsm.unregisterUtility(provided=IBrowserSkinType,
-                                        name=self._skin_name)
+            res = gsm.unregisterUtility(provided=IBrowserSkinType, name=self._skin_name)
             self.assertTrue(res)
             if self._old_theme_layer is not None:
-                gsm.registerUtility(self._old_theme_layer,
-                                    IBrowserSkinType,
-                                    self._skin_name)
+                gsm.registerUtility(
+                    self._old_theme_layer, IBrowserSkinType, self._skin_name
+                )
 
 
 class TestPrecedenceWithAdditiveLayerExtendingInterface(LayerPrecedenceTestCase):
     theme_layer = IThemeSpecific
     additive_layer = IAdditiveLayer
 
 
@@ -99,13 +97,15 @@
 
 class TestPrecedenceWithNoThemeLayer(LayerPrecedenceTestCase):
     theme_layer = None
     additive_layer = IAdditiveLayer
 
 
 def test_suite():
-    from unittest import TestSuite, makeSuite
+    from unittest import makeSuite
+    from unittest import TestSuite
+
     suite = TestSuite()
     suite.addTest(makeSuite(TestPrecedenceWithAdditiveLayerExtendingInterface))
     suite.addTest(makeSuite(TestPrecedenceWithAdditiveLayerExtendingDefault))
     suite.addTest(makeSuite(TestPrecedenceWithNoThemeLayer))
     return suite
```

### Comparing `plone.theme-3.0.7/plone/theme/layer.py` & `plone.theme-4.0.0/plone/theme/layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# -*- coding: utf-8 -*-
 from plone.theme.interfaces import IDefaultPloneLayer
 from Products.CMFCore.utils import getToolByName
 from zope.component import queryUtility
-from zope.interface import directlyProvides, directlyProvidedBy
+from zope.interface import directlyProvidedBy
+from zope.interface import directlyProvides
 from zope.publisher.interfaces.browser import IBrowserSkinType
 from zope.publisher.interfaces.browser import IDefaultBrowserLayer
 
+
 default_layers = [
     IDefaultPloneLayer,
     IDefaultBrowserLayer,
-    ]
+]
 
 
 def mark_layer(site, event):
     """Mark the request with a layer corresponding to the current skin,
     as set in the portal_skins tool.
     """
-    if getattr(event.request, '_plonetheme_', False):
+    if getattr(event.request, "_plonetheme_", False):
         return
     event.request._plonetheme_ = True
 
-    portal_skins = getToolByName(site, 'portal_skins', None)
+    portal_skins = getToolByName(site, "portal_skins", None)
     if portal_skins is not None:
         skin_name = site.getCurrentSkinName()
         if skin_name is None:
             return
         skin = queryUtility(IBrowserSkinType, name=skin_name)
         if skin is not None:
             layer_ifaces = []
@@ -36,9 +37,15 @@
             for layer in directlyProvidedBy(event.request):
                 if layer in default_layers:
                     default_ifaces.append(layer)
                 elif IBrowserSkinType.providedBy(layer):
                     continue
                 else:
                     layer_ifaces.append(layer)
-            ifaces = [skin, ] + layer_ifaces + default_ifaces
+            ifaces = (
+                [
+                    skin,
+                ]
+                + layer_ifaces
+                + default_ifaces
+            )
             directlyProvides(event.request, *ifaces)
```

### Comparing `plone.theme-3.0.7/plone/theme/README.rst` & `plone.theme-4.0.0/plone/theme/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -64,27 +64,30 @@
     >>> from plone.testing.z2 import Browser
     >>> browser = Browser(layer['app'])
 
     >>> browser.open(layer['portal'].absolute_url() + '/@@layer-test-view')
     >>> from __future__ import print_function
     >>> print(browser.contents)
     Default
+    ...
 
 However, if we turn the skin on, we should see the effects of the marker
 interface being applied.
 
     >>> portal_skins.default_skin = 'My Theme'
     >>> import transaction
     >>> transaction.commit()
 
     >>> browser.open(layer['portal'].absolute_url() + '/@@layer-test-view')
     >>> print(browser.contents)
     My Theme
+    ...
 
 And if we switch back:
 
     >>> portal_skins.default_skin = 'Plone Default'
     >>> transaction.commit()
 
     >>> browser.open(layer['portal'].absolute_url() + '/@@layer-test-view')
     >>> print(browser.contents)
     Default
+    ...
```

### Comparing `plone.theme-3.0.7/plone/theme/testing.py` & `plone.theme-4.0.0/plone/theme/testing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# -*- coding: utf-8 -*-
-
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing.layers import FunctionalTesting
 from plone.app.testing.layers import IntegrationTesting
 
 
 class PloneThemeLayer(PloneSandboxLayer):
-
     def setUpZope(self, app, configurationContext):
         import plone.theme.tests
-        self.loadZCML('tests.zcml', package=plone.theme.tests)
+
+        self.loadZCML("tests.zcml", package=plone.theme.tests)
+
 
 PLONETHEME_FIXTURE = PloneThemeLayer()
 
 PLONETHEME_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(PLONETHEME_FIXTURE,),
-    name="PloneTheme:Functional")
+    bases=(PLONETHEME_FIXTURE,), name="PloneTheme:Functional"
+)
 
 PLONETHEME_INTEGRATION_TESTING = IntegrationTesting(
-    bases=(PLONETHEME_FIXTURE,),
-    name="PloneTheme:Integration")
+    bases=(PLONETHEME_FIXTURE,), name="PloneTheme:Integration"
+)
```

### Comparing `plone.theme-3.0.7/CHANGES.rst` & `plone.theme-4.0.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.0 (2023-04-27)
+------------------
+
+Breaking changes:
+
+
+- Drop Python 2 and Plone 5.2 support.
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
 3.0.7 (2020-04-22)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
```

