# Comparing `tmp/plone.resourceeditor-3.0.4.tar.gz` & `tmp/plone.resourceeditor-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.resourceeditor-3.0.4.tar", last modified: Tue Aug 30 11:58:57 2022, max compression
+gzip compressed data, was "plone.resourceeditor-4.0.0.tar", last modified: Wed Apr 26 22:03:36 2023, max compression
```

## Comparing `plone.resourceeditor-3.0.4.tar` & `plone.resourceeditor-4.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.836107 plone.resourceeditor-3.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)     3639 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5399 2022-08-30 11:58:57.836201 plone.resourceeditor-3.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      835 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.831679 plone.resourceeditor-3.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      729 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.831889 plone.resourceeditor-3.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.835218 plone.resourceeditor-3.0.4/plone/resourceeditor/
--rw-r--r--   0 maurits    (501) staff       (20)      479 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    43230 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1646 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1108 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/editor.pt
--rw-r--r--   0 maurits    (501) staff       (20)       21 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/mime.types
--rw-r--r--   0 maurits    (501) staff       (20)      850 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/preview.pt
--rw-r--r--   0 maurits    (501) staff       (20)      886 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.835919 plone.resourceeditor-3.0.4/plone/resourceeditor/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    12942 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/tests/test_file_manager.py
--rw-r--r--   0 maurits    (501) staff       (20)    11844 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone/resourceeditor/tests/test_file_manager_action.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-08-30 11:58:57.833624 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     5399 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      822 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      126 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2022-08-30 11:58:57.836537 plone.resourceeditor-3.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1560 2022-08-30 11:58:57.000000 plone.resourceeditor-3.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:36.248579 plone.resourceeditor-4.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     3820 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5466 2023-04-26 22:03:36.248685 plone.resourceeditor-4.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      835 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:36.243504 plone.resourceeditor-4.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      729 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:36.243768 plone.resourceeditor-4.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:36.247594 plone.resourceeditor-4.0.0/plone/resourceeditor/
+-rw-r--r--   0 maurits    (501) staff       (20)      455 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    40960 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1573 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1234 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/editor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       21 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/mime.types
+-rw-r--r--   0 maurits    (501) staff       (20)      887 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/preview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      838 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:36.248361 plone.resourceeditor-4.0.0/plone/resourceeditor/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12917 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/tests/test_file_manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11832 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/plone/resourceeditor/tests/test_file_manager_action.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:03:36.245758 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     5466 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      822 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:03:36.000000 plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2906 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 22:03:36.249102 plone.resourceeditor-4.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1389 2023-04-26 22:03:35.000000 plone.resourceeditor-4.0.0/setup.py
```

### Comparing `plone.resourceeditor-3.0.4/CHANGES.rst` & `plone.resourceeditor-4.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

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
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (2a4ba395)
+
+
 3.0.4 (2022-08-30)
 ------------------
 
 Bug fixes:
 
 
 - Fix unclosed file warnings
@@ -107,15 +124,15 @@
 ------------------
 
 Fixes:
 
 - Remove  unittest2 dependency
   [kakshay21]
 - Split the error message for the move API endpoint into two. One
-  is for the parent folder and the other is for the distination folder
+  is for the parent folder and the other is for the destination folder
   [b4oshany]
 - Fix Jenkins flake8 errors
 
 
 [b4oshany]: https://github.com/b4oshany
 
 2.0.5 (2016-03-31)
@@ -156,15 +173,15 @@
 - handle NotFound errors while generating file/folder listings
   [vangheem]
 
 
 2.0.2 (2015-09-08)
 ------------------
 
-- Added check to prevent overwritting folders when saving
+- Added check to prevent overwriting folders when saving
   [obct537]
 
 2.0.1 (2015-08-22)
 ------------------
 
 - Added ability to convert absolute to relative urls
   [obct537]
```

### Comparing `plone.resourceeditor-3.0.4/PKG-INFO` & `plone.resourceeditor-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: plone.resourceeditor
-Version: 3.0.4
+Version: 4.0.0
 Summary: Integrates ACE editor into Plone
 Home-page: https://github.com/plone/plone.resourceeditor
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: ace resource editor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 This package contains resources for integrating `ACE embeddable code editor <http://ace.ajax.org>`_ into Plone.
 It provides a file manager that can edit ``plone.resource`` resource directories in the ZODB.
@@ -54,14 +52,31 @@
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
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (2a4ba395)
+
+
 3.0.4 (2022-08-30)
 ------------------
 
 Bug fixes:
 
 
 - Fix unclosed file warnings
@@ -157,15 +172,15 @@
 ------------------
 
 Fixes:
 
 - Remove  unittest2 dependency
   [kakshay21]
 - Split the error message for the move API endpoint into two. One
-  is for the parent folder and the other is for the distination folder
+  is for the parent folder and the other is for the destination folder
   [b4oshany]
 - Fix Jenkins flake8 errors
 
 
 [b4oshany]: https://github.com/b4oshany
 
 2.0.5 (2016-03-31)
@@ -206,15 +221,15 @@
 - handle NotFound errors while generating file/folder listings
   [vangheem]
 
 
 2.0.2 (2015-09-08)
 ------------------
 
-- Added check to prevent overwritting folders when saving
+- Added check to prevent overwriting folders when saving
   [obct537]
 
 2.0.1 (2015-08-22)
 ------------------
 
 - Added ability to convert absolute to relative urls
   [obct537]
```

### Comparing `plone.resourceeditor-3.0.4/README.rst` & `plone.resourceeditor-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.resourceeditor-3.0.4/docs/LICENSE.GPL` & `plone.resourceeditor-4.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.resourceeditor-3.0.4/docs/LICENSE.txt` & `plone.resourceeditor-4.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.resourceeditor-3.0.4/plone/resourceeditor/browser.py` & `plone.resourceeditor-4.0.0/plone/resourceeditor/browser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,66 @@
-# -*- coding: utf-8 -*-
 from AccessControl import Unauthorized
 from DateTime import DateTime
 from OFS.Image import File
 from OFS.Image import Image
+from plone.base.utils import safe_text
 from plone.resource.directory import FilesystemResourceDirectory
 from plone.resource.file import FilesystemFile
 from plone.resource.interfaces import IResourceDirectory
 from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.utils import safe_unicode
-from Products.CMFPlone.utils import safe_encode
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
-from six.moves import urllib
-from six.moves.urllib.parse import urlparse
 from time import localtime
 from time import strftime
+from urllib.parse import urlparse
 from zExceptions import NotFound
 from zope.cachedescriptors import property as zproperty
 from zope.component import queryMultiAdapter
 from zope.component.hooks import getSite
 from zope.i18n import translate
 from zope.i18nmessageid import MessageFactory
 from zope.publisher.browser import BrowserView
 
 import json
 import os.path
 import posixpath
 import re
-import six
+import urllib
 
 
-_ = MessageFactory(u'plone')
+_ = MessageFactory("plone")
 
 
 def authorize(context, request):
-    authenticator = queryMultiAdapter((context, request),
-                                      name=u'authenticator')
+    authenticator = queryMultiAdapter((context, request), name="authenticator")
     if authenticator is not None and not authenticator.verify():
         raise Unauthorized
 
 
 invalidFilenameChars = frozenset(r'\/:*?"<>|')
 
 
 def validateFilename(name):
     return len([n for n in name if n in invalidFilenameChars]) == 0
 
 
 class FileManagerActions(BrowserView):
-
-    imageExtensions = ['png', 'gif', 'jpg', 'jpeg', 'ico']
-    previewTemplate = ViewPageTemplateFile('preview.pt')
+    imageExtensions = ["png", "gif", "jpg", "jpeg", "ico"]
+    previewTemplate = ViewPageTemplateFile("preview.pt")
 
     @zproperty.Lazy
     def resourceDirectory(self):
         return self.context
 
     def getObject(self, path):
         path = self.normalizePath(path)
         if not path:
             return self.resourceDirectory
         try:
             return self.resourceDirectory[path]
-        except (KeyError, NotFound,):
+        except (KeyError, NotFound):
             raise KeyError(path)
 
     def getExtension(self, obj=None, path=None):
         if not path:
             path = obj.__name__
         basename, ext = os.path.splitext(path)
         ext = ext[1:].lower()
@@ -82,681 +77,697 @@
 
         Optionally a "type" parameter can be specified to restrict returned
         files (depending on the connector). If a "type" parameter is given for
         the HTML document, the same parameter value is reused and passed
         to getFolder(). This can be used for example to only show image files
         in a file system tree.
         """
-        if six.PY2 and isinstance(path, six.text_type):
-            path = safe_encode(path, 'utf-8')
-
         folders = []
         files = []
 
         path = self.normalizePath(path)
         folder = self.getObject(path)
 
         for name in folder.listDirectory():
             if IResourceDirectory.providedBy(folder[name]):
-                folders.append(self.getInfo(
-                    folder[name],
-                    path='/{0}/{1}/'.format(path, name)
-                ))
+                folders.append(self.getInfo(folder[name], path=f"/{path}/{name}/"))
             else:
-                files.append(self.getInfo(
-                    folder[name],
-                    path='/{0}/{1}'.format(path, name)
-                ))
+                files.append(self.getInfo(folder[name], path=f"/{path}/{name}"))
         return folders + files
 
     def getFile(self, path):
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
         path = self.normalizePath(path)
         ext = self.getExtension(path=path)
-        result = {'ext': ext}
-        self.request.response.setHeader('Content-Type', 'application/json')
+        result = {"ext": ext}
+        self.request.response.setHeader("Content-Type", "application/json")
 
         if ext in self.imageExtensions:
             obj = self.getObject(path)
             info = self.getInfo(obj)
-            info['preview'] = path
-            result['info'] = self.previewTemplate(info=info)
+            info["preview"] = path
+            result["info"] = self.previewTemplate(info=info)
             return json.dumps(result)
         else:
             try:
                 data = self.context.readFile(path)
 
-                if six.PY2 and isinstance(data, six.text_type):
-                    result['contents'] = data.encode('utf8')
-                else:
-                    result['contents'] = safe_unicode(data)
+                result["contents"] = safe_text(data)
                 try:
                     return json.dumps(result)
                 except UnicodeDecodeError:
                     # The file we're trying to get isn't unicode encodable
                     # so we just return the file information, not the content
-                    del result['contents']
+                    del result["contents"]
                     obj = self.getObject(path)
                     info = self.getInfo(obj)
-                    result['info'] = self.previewTemplate(info=info)
+                    result["info"] = self.previewTemplate(info=info)
                     return json.dumps(result)
             except AttributeError:
                 return None
 
     def normalizePath(self, path):
-        if path.startswith('/'):
+        if path.startswith("/"):
             path = path[1:]
-        if path.endswith('/'):
+        if path.endswith("/"):
             path = path[:-1]
         return path
 
     def normalizeReturnPath(self, path):
-        if path.endswith('/'):
+        if path.endswith("/"):
             path = path[:-1]
-        if not path.startswith('/'):
-            path = '/' + path
+        if not path.startswith("/"):
+            path = "/" + path
         return path
 
     def parentPath(self, path):
-        return '/'.join(path.split('/')[:-1])
+        return "/".join(path.split("/")[:-1])
 
-    def getInfo(self, obj, path='/'):
+    def getInfo(self, obj, path="/"):
         """Returns information about a single file. Requests
         with mode "getinfo" will include an additional parameter, "path",
         indicating which file to inspect. A boolean parameter "getsize"
         indicates whether the dimensions of the file (if an image) should be
         returned.
         """
         filename = obj.__name__
 
         properties = {
-            'dateModified': None,
+            "dateModified": None,
         }
 
         size = 0
 
         if isinstance(obj, File):
-            properties['dateModified'] = DateTime(obj._p_mtime).strftime('%c')
+            properties["dateModified"] = DateTime(obj._p_mtime).strftime("%c")
             size = obj.get_size() / 1024
 
         if IResourceDirectory.providedBy(obj):
-            fileType = 'dir'
+            fileType = "dir"
             is_folder = True
         else:
             fileType = self.getExtension(obj)
             is_folder = False
         if isinstance(obj, FilesystemFile):
             stats = os.stat(obj.path)
             modified = localtime(stats.st_mtime)
-            properties['dateModified'] = strftime('%c', modified)
+            properties["dateModified"] = strftime("%c", modified)
             size = stats.st_size / 1024
 
         if size < 1024:
-            size_specifier = u'kb'
+            size_specifier = "kb"
         else:
-            size_specifier = u'mb'
+            size_specifier = "mb"
             size = size / 1024
-        properties['size'] = '{0}{1}'.format(
+        properties["size"] = "{}{}".format(
             size,
-            translate(_(u'filemanager_{0}'.format(size_specifier),
-                        default=size_specifier), context=self.request)
+            translate(
+                _(f"filemanager_{size_specifier}", default=size_specifier),
+                context=self.request,
+            ),
         )
 
         if isinstance(obj, Image):
-            properties['height'] = obj.height
-            properties['width'] = obj.width
+            properties["height"] = obj.height
+            properties["width"] = obj.width
 
         return {
-            'filename': filename,
-            'label': filename,
-            'fileType': fileType,
-            'filesystem': isinstance(obj, FilesystemFile),
-            'properties': properties,
-            'path': path,
-            'folder': is_folder
+            "filename": filename,
+            "label": filename,
+            "fileType": fileType,
+            "filesystem": isinstance(obj, FilesystemFile),
+            "properties": properties,
+            "path": path,
+            "folder": is_folder,
         }
 
     def saveFile(self, path, value):
-        path = path.lstrip('/')
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-        value = value.strip()
-        if six.PY2:
-            value = safe_encode(value, 'utf-8')
-
-        value = value.replace('\r\n', '\n')
+        path = path.lstrip("/")
+        value = value.strip().replace("\r\n", "\n")
 
         if path in self.context:
             if IResourceDirectory.providedBy(self.context[path]):
-                return json.dumps({'error': 'invalid path'})
+                return json.dumps({"error": "invalid path"})
 
-        if 'relativeUrls' in self.request.form:
-            reg = re.compile(r'url\(([^)]+)\)')
+        if "relativeUrls" in self.request.form:
+            reg = re.compile(r"url\(([^)]+)\)")
             urls = reg.findall(value)
 
             # Trim off the @@plone.resourceeditor bit to just give us the
             # theme url
-            limit = self.request.URL.find('@@plone.resourceeditor')
+            limit = self.request.URL.find("@@plone.resourceeditor")
             location = self.request.URL[0:limit]
             base = urlparse(location)
             for url in urls:
                 asset = urlparse(url.strip("'").strip('"'))
                 if base.netloc != asset.netloc:
                     continue
 
-                base_dir = '.' + posixpath.dirname(base.path)
-                target = '.' + asset.path
+                base_dir = "." + posixpath.dirname(base.path)
+                target = "." + asset.path
                 out = posixpath.relpath(target, start=base_dir)
                 value = value.replace(url.strip('"').strip("'"), out)
 
-        self.request.response.setHeader('Content-Type', 'application/json')
+        self.request.response.setHeader("Content-Type", "application/json")
         if isinstance(self.context, FilesystemResourceDirectory):
             # we cannot save in an FS directory, but we return the file content
             # (useful when we compile less from the theming editor)
-            return json.dumps({'success': 'tmp', 'value': value})
+            return json.dumps({"success": "tmp", "value": value})
         else:
             self.context.writeFile(path, value)
-            return json.dumps({'success': 'save'})
+            return json.dumps({"success": "save"})
 
     def addFolder(self, path, name):
-        """Create a new directory on the server within the given path.
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            name = safe_encode(name, 'utf-8')
-
+        """Create a new directory on the server within the given path."""
         code = 0
-        error = ''
+        error = ""
 
         parentPath = self.normalizePath(path)
         parent = None
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if not validateFilename(name):
-                error = translate(_(u'filemanager_invalid_foldername',
-                                  default=u'Invalid folder name.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_invalid_foldername", default="Invalid folder name."),
+                    context=self.request,
+                )
                 code = 1
             elif name in parent:
-                error = translate(_(u'filemanager_error_folder_exists',
-                                  default=u'Folder already exists.'),
-                                  context=self.request)
+                error = translate(
+                    _(
+                        "filemanager_error_folder_exists",
+                        default="Folder already exists.",
+                    ),
+                    context=self.request,
+                )
                 code = 1
             else:
                 try:
                     parent.makeDirectory(name)
                 except UnicodeDecodeError:
                     error = translate(
                         _(
-                            u'filemanager_invalid_foldername',
-                            default=u'Invalid folder name.'
+                            "filemanager_invalid_foldername",
+                            default="Invalid folder name.",
                         ),
-                        context=self.request
+                        context=self.request,
                     )
                     code = 1
 
-        self.request.response.setHeader('Content-Type', 'application/json')
-        return json.dumps({
-            'parent': self.normalizeReturnPath(parentPath),
-            'name': name,
-            'error': error,
-            'code': code,
-        })
+        self.request.response.setHeader("Content-Type", "application/json")
+        return json.dumps(
+            {
+                "parent": self.normalizeReturnPath(parentPath),
+                "name": name,
+                "error": error,
+                "code": code,
+            }
+        )
 
     def addFile(self, path, name):
-        """Add a new empty file in the given directory
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            name = safe_encode(name, 'utf-8')
-
-        error = ''
+        """Add a new empty file in the given directory"""
+        error = ""
         code = 0
 
         parentPath = self.normalizePath(path)
-        newPath = '{0}/{1}'.format(parentPath, name,)
+        newPath = f"{parentPath}/{name}"
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if not validateFilename(name):
-                error = translate(_(u'filemanager_invalid_filename',
-                                  default=u'Invalid file name.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_invalid_filename", default="Invalid file name."),
+                    context=self.request,
+                )
                 code = 1
             elif name in parent:
-                error = translate(_(u'filemanager_error_file_exists',
-                                  default=u'File already exists.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_error_file_exists", default="File already exists."),
+                    context=self.request,
+                )
                 code = 1
             else:
-                self.resourceDirectory.writeFile(newPath, b'')
+                self.resourceDirectory.writeFile(newPath, b"")
 
-        self.request.response.setHeader('Content-Type', 'application/json')
-        return json.dumps({
-            'parent': self.normalizeReturnPath(parentPath),
-            'name': name,
-            'error': error,
-            'code': code,
-            'path': path
-        })
+        self.request.response.setHeader("Content-Type", "application/json")
+        return json.dumps(
+            {
+                "parent": self.normalizeReturnPath(parentPath),
+                "name": name,
+                "error": error,
+                "code": code,
+                "path": path,
+            }
+        )
 
     def delete(self, path):
-        """Delete the item at the given path.
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
+        """Delete the item at the given path."""
         npath = self.normalizePath(path)
-        parentPath = '/'.join(npath.split('/')[:-1])
-        name = npath.split('/')[-1]
+        parentPath = "/".join(npath.split("/")[:-1])
+        name = npath.split("/")[-1]
         code = 0
-        error = ''
+        error = ""
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             try:
                 del parent[name]
             except KeyError:
-                error = translate(_(u'filemanager_error_file_not_found',
-                                  default=u'File not found.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_error_file_not_found", default="File not found."),
+                    context=self.request,
+                )
                 code = 1
 
-        self.request.response.setHeader('Content-Type', 'application/json')
-        return json.dumps({
-            'path': self.normalizeReturnPath(path),
-            'error': error,
-            'code': code,
-        })
+        self.request.response.setHeader("Content-Type", "application/json")
+        return json.dumps(
+            {
+                "path": self.normalizeReturnPath(path),
+                "error": error,
+                "code": code,
+            }
+        )
 
     def renameFile(self, path, newName):
-        """Rename the item at the given path to the new name
-        """
-
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            newName = safe_encode(newName, 'utf-8')
-
+        """Rename the item at the given path to the new name"""
         npath = self.normalizePath(path)
-        oldPath = newPath = '/'.join(npath.split('/')[:-1])
-        oldName = npath.split('/')[-1]
+        oldPath = newPath = "/".join(npath.split("/")[:-1])
+        oldName = npath.split("/")[-1]
 
         code = 0
-        error = ''
+        error = ""
 
         try:
             parent = self.getObject(oldPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if newName != oldName:
                 if newName in parent:
                     error = translate(
                         _(
-                            u'filemanager_error_file_exists',
-                            default=u'File already exists.'
+                            "filemanager_error_file_exists",
+                            default="File already exists.",
                         ),
-                        context=self.request)
+                        context=self.request,
+                    )
                     code = 1
                 else:
                     parent.rename(oldName, newName)
 
-        self.request.response.setHeader('Content-Type', 'application/json')
-        return json.dumps({
-            'oldParent': self.normalizeReturnPath(oldPath),
-            'oldName': oldName,
-            'newParent': self.normalizeReturnPath(newPath),
-            'newName': newName,
-            'error': error,
-            'code': code,
-        })
+        self.request.response.setHeader("Content-Type", "application/json")
+        return json.dumps(
+            {
+                "oldParent": self.normalizeReturnPath(oldPath),
+                "oldName": oldName,
+                "newParent": self.normalizeReturnPath(newPath),
+                "newName": newName,
+                "error": error,
+                "code": code,
+            }
+        )
 
     def move(self, path, directory):
-        """Move the item at the given path to a new directory
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            directory = safe_encode(directory, 'utf-8')
-
+        """Move the item at the given path to a new directory"""
         npath = self.normalizePath(path)
         newParentPath = self.normalizePath(directory)
 
         parentPath = self.parentPath(npath)
-        filename = npath.split('/')[-1]
+        filename = npath.split("/")[-1]
 
         code = 0
-        error = ''
-        newCanonicalPath = '{0}/{1}'.format(newParentPath, filename)
+        error = ""
+        newCanonicalPath = f"{newParentPath}/{filename}"
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
-            return json.dumps({
-                'code': code,
-                'error': error,
-                'newPath': self.normalizeReturnPath(newCanonicalPath),
-            })
+            return json.dumps(
+                {
+                    "code": code,
+                    "error": error,
+                    "newPath": self.normalizeReturnPath(newCanonicalPath),
+                }
+            )
 
         try:
             target = self.getObject(newParentPath)
         except KeyError:
-            error = translate(_(u'filemanager_error_folder_exists',
-                              default=u'Destination folder not found.'),
-                              context=self.request)
+            error = translate(
+                _(
+                    "filemanager_error_folder_exists",
+                    default="Destination folder not found.",
+                ),
+                context=self.request,
+            )
             code = 1
-            return json.dumps({
-                'code': code,
-                'error': error,
-                'newPath': self.normalizeReturnPath(newCanonicalPath),
-            })
+            return json.dumps(
+                {
+                    "code": code,
+                    "error": error,
+                    "newPath": self.normalizeReturnPath(newCanonicalPath),
+                }
+            )
 
         if filename not in parent:
-            error = translate(_(u'filemanager_error_file_not_found',
-                              default=u'File not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_error_file_not_found", default="File not found."),
+                context=self.request,
+            )
             code = 1
         elif filename in target:
-            error = translate(_(u'filemanager_error_file_exists',
-                              default=u'File already exists.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_error_file_exists", default="File already exists."),
+                context=self.request,
+            )
             code = 1
         else:
             obj = parent[filename]
             del parent[filename]
             target[filename] = obj
 
-        return json.dumps({
-            'code': code,
-            'error': error,
-            'newPath': self.normalizeReturnPath(newCanonicalPath),
-        })
+        return json.dumps(
+            {
+                "code": code,
+                "error": error,
+                "newPath": self.normalizeReturnPath(newCanonicalPath),
+            }
+        )
 
     def do_action(self, action):
-        if action == 'dataTree':
+        if action == "dataTree":
 
-            def getDirectory(folder, relpath=''):
+            def getDirectory(folder, relpath=""):
                 items = []
                 for name in folder.listDirectory():
                     obj = folder[name]
-                    path = relpath + '/' + name
+                    path = relpath + "/" + name
                     if IResourceDirectory.providedBy(obj):
                         try:
                             children = getDirectory(obj, path)
                         except NotFound:
                             children = []
-                        items.append({
-                            'label': name,
-                            'folder': True,
-                            'path': path,
-                            'children': children
-                        })
+                        items.append(
+                            {
+                                "label": name,
+                                "folder": True,
+                                "path": path,
+                                "children": children,
+                            }
+                        )
                     else:
                         items.append(self.getInfo(obj, path))
                 return items
 
             return json.dumps(getDirectory(self.context))
 
-        if action == 'getFile':
-            path = self.request.get('path', '')
+        if action == "getFile":
+            path = self.request.get("path", "")
             return self.getFile(path)
 
-        if action == 'saveFile':
-            path = self.request.get('path', '')
-            data = self.request.get('data', '')
+        if action == "saveFile":
+            path = self.request.get("path", "")
+            data = self.request.get("data", "")
             return self.saveFile(path, data)
 
-        if action == 'addFolder':
-            path = self.request.get('path', '')
-            name = self.request.get('name', '')
+        if action == "addFolder":
+            path = self.request.get("path", "")
+            name = self.request.get("name", "")
             return self.addFolder(path, name)
 
-        if action == 'addFile':
-            path = self.request.get('path', '')
-            name = self.request.get('filename', '')
+        if action == "addFile":
+            path = self.request.get("path", "")
+            name = self.request.get("filename", "")
             return self.addFile(path, name)
 
-        if action == 'renameFile':
-            path = self.request.get('path', '')
-            name = self.request.get('filename', '')
+        if action == "renameFile":
+            path = self.request.get("path", "")
+            name = self.request.get("filename", "")
             return self.renameFile(path, name)
 
-        if action == 'delete':
-            path = self.request.get('path', '')
+        if action == "delete":
+            path = self.request.get("path", "")
             return self.delete(path)
 
-        if action == 'move':
-            src_path = self.request.get('source', '')
-            des_path = self.request.get('destination', '')
+        if action == "move":
+            src_path = self.request.get("source", "")
+            des_path = self.request.get("destination", "")
             return self.move(src_path, des_path)
 
     def download(self, path):
-        """Serve the requested file to the user
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
+        """Serve the requested file to the user"""
         npath = self.normalizePath(path)
-        parentPath = '/'.join(npath.split('/')[:-1])
-        name = npath.split('/')[-1]
+        parentPath = "/".join(npath.split("/")[:-1])
+        name = npath.split("/")[-1]
 
         parent = self.getObject(parentPath)
 
-        self.request.response.setHeader('Content-Type',
-                                        'application/octet-stream')
+        self.request.response.setHeader("Content-Type", "application/octet-stream")
         self.request.response.setHeader(
-            'Content-Disposition',
-            'attachment; filename="{0}"'.format(name)
+            "Content-Disposition", f'attachment; filename="{name}"'
         )
 
         # TODO: Use streams here if we can
         return parent.readFile(name)
 
     def __call__(self):
-        action = self.request.get('action')
+        action = self.request.get("action")
         return self.do_action(action)
 
 
 class FileManager(BrowserView):
-    """Render the file manager and support its AJAX requests.
-    """
+    """Render the file manager and support its AJAX requests."""
 
-    previewTemplate = ViewPageTemplateFile('preview.pt')
-    staticFiles = '++resource++plone.resourceeditor/filemanager'
-    imageExtensions = ['png', 'gif', 'jpg', 'jpeg']
-    knownExtensions = ['css', 'html', 'htm', 'txt', 'xml', 'js', 'cfg']
-    capabilities = ['download', 'rename', 'delete']
-
-    extensionsWithIcons = frozenset([
-        'aac', 'avi', 'bmp', 'chm', 'css', 'dll', 'doc', 'fla',
-        'gif', 'htm', 'html', 'ini', 'jar', 'jpeg', 'jpg', 'js',
-        'lasso', 'mdb', 'mov', 'mp3', 'mpg', 'pdf', 'php', 'png',
-        'ppt', 'py', 'rb', 'real', 'reg', 'rtf', 'sql', 'swf', 'txt',
-        'vbs', 'wav', 'wma', 'wmv', 'xls', 'xml', 'xsl', 'zip',
-    ])
-
-    protectedActions = (
-        'addfolder', 'add', 'addnew',
-        'rename', 'delete'
+    previewTemplate = ViewPageTemplateFile("preview.pt")
+    staticFiles = "++resource++plone.resourceeditor/filemanager"
+    imageExtensions = ["png", "gif", "jpg", "jpeg"]
+    knownExtensions = ["css", "html", "htm", "txt", "xml", "js", "cfg"]
+    capabilities = ["download", "rename", "delete"]
+
+    extensionsWithIcons = frozenset(
+        [
+            "aac",
+            "avi",
+            "bmp",
+            "chm",
+            "css",
+            "dll",
+            "doc",
+            "fla",
+            "gif",
+            "htm",
+            "html",
+            "ini",
+            "jar",
+            "jpeg",
+            "jpg",
+            "js",
+            "lasso",
+            "mdb",
+            "mov",
+            "mp3",
+            "mpg",
+            "pdf",
+            "php",
+            "png",
+            "ppt",
+            "py",
+            "rb",
+            "real",
+            "reg",
+            "rtf",
+            "sql",
+            "swf",
+            "txt",
+            "vbs",
+            "wav",
+            "wma",
+            "wmv",
+            "xls",
+            "xml",
+            "xsl",
+            "zip",
+        ]
     )
 
+    protectedActions = ("addfolder", "add", "addnew", "rename", "delete")
+
     def pattern_options(self):
         site = getSite()
-        viewName = '@@plone.resourceeditor.filemanager-actions'
-        return json.dumps({
-            'actionUrl': '{0}/++{1}++{2}/{3}'.format(
-                site.absolute_url(),
-                self.context.__parent__.__parent__.__name__,
-                self.context.__name__,
-                viewName
-            )
-        })
+        viewName = "@@plone.resourceeditor.filemanager-actions"
+        return json.dumps(
+            {
+                "actionUrl": "{}/++{}++{}/{}".format(
+                    site.absolute_url(),
+                    self.context.__parent__.__parent__.__name__,
+                    self.context.__name__,
+                    viewName,
+                )
+            }
+        )
 
     def mode_selector(self, form):
         # AJAX methods called by the file manager
-        mode = form['mode']
+        mode = form["mode"]
 
         if mode in self.protectedActions:
             authorize(self.context, self.request)
 
-        response = {'error:': 'Unknown request', 'code': -1}
+        response = {"error:": "Unknown request", "code": -1}
         textareaWrap = False
 
-        if mode == u'getfolder':
+        if mode == "getfolder":
             response = self.getFolder(
-                path=urllib.parse.unquote(form['path']),
-                getSizes=form.get('getsizes', 'false') == 'true'
+                path=urllib.parse.unquote(form["path"]),
+                getSizes=form.get("getsizes", "false") == "true",
             )
-        elif mode == u'getinfo':
+        elif mode == "getinfo":
             response = self.getInfo(
-                path=urllib.parse.unquote(form['path']),
-                getSize=form.get('getsize', 'false') == 'true'
+                path=urllib.parse.unquote(form["path"]),
+                getSize=form.get("getsize", "false") == "true",
             )
-        elif mode == u'addfolder':
+        elif mode == "addfolder":
             response = self.addFolder(
-                path=urllib.parse.unquote(form['path']),
-                name=urllib.parse.unquote(form['name'])
+                path=urllib.parse.unquote(form["path"]),
+                name=urllib.parse.unquote(form["name"]),
             )
-        elif mode == u'add':
+        elif mode == "add":
             textareaWrap = True
             response = self.add(
-                path=urllib.parse.unquote(form['currentpath']),
-                newfile=form['newfile'],
-                replacepath=form.get('replacepath', None)
+                path=urllib.parse.unquote(form["currentpath"]),
+                newfile=form["newfile"],
+                replacepath=form.get("replacepath", None),
             )
-        elif mode == u'addnew':
+        elif mode == "addnew":
             response = self.addNew(
-                path=urllib.parse.unquote(form['path']),
-                name=urllib.parse.unquote(form['name'])
+                path=urllib.parse.unquote(form["path"]),
+                name=urllib.parse.unquote(form["name"]),
             )
-        elif mode == u'rename':
+        elif mode == "rename":
             response = self.rename(
-                path=urllib.parse.unquote(form['old']),
-                newName=urllib.parse.unquote(form['new'])
-            )
-        elif mode == u'delete':
-            response = self.delete(
-                path=urllib.parse.unquote(form['path'])
+                path=urllib.parse.unquote(form["old"]),
+                newName=urllib.parse.unquote(form["new"]),
             )
-        elif mode == 'move':
+        elif mode == "delete":
+            response = self.delete(path=urllib.parse.unquote(form["path"]))
+        elif mode == "move":
             response = self.move(
-                path=urllib.parse.unquote(form['path']),
-                directory=urllib.parse.unquote(form['directory'])
-            )
-        elif mode == u'download':
-            return self.download(
-                path=urllib.parse.unquote(form['path'])
+                path=urllib.parse.unquote(form["path"]),
+                directory=urllib.parse.unquote(form["directory"]),
             )
+        elif mode == "download":
+            return self.download(path=urllib.parse.unquote(form["path"]))
         if textareaWrap:
-            self.request.response.setHeader('Content-Type', 'text/html')
-            return '<textarea>{0}</textarea>'.format(json.dumps(response))
-        self.request.response.setHeader('Content-Type',
-                                        'application/json')
+            self.request.response.setHeader("Content-Type", "text/html")
+            return f"<textarea>{json.dumps(response)}</textarea>"
+        self.request.response.setHeader("Content-Type", "application/json")
         return json.dumps(response)
 
     def __call__(self):
         # make sure theme is disable for these requests
-        self.request.response.setHeader('X-Theme-Disabled', 'True')
-        self.request['HTTP_X_THEME_ENABLED'] = False
+        self.request.response.setHeader("X-Theme-Disabled", "True")
+        self.request["HTTP_X_THEME_ENABLED"] = False
 
         self.setup()
         form = self.request.form
 
         # AJAX methods called by the file manager
-        if 'mode' in form:
+        if "mode" in form:
             return self.mode_selector(form)
 
         # Rendering the view
         else:
             return self.index()
 
     def setup(self):
         pass
 
     @zproperty.Lazy
     def portalUrl(self):
-        return getToolByName(self.context, 'portal_url')()
+        return getToolByName(self.context, "portal_url")()
 
     @zproperty.Lazy
     def resourceDirectory(self):
         return self.context
 
     @zproperty.Lazy
     def resourceType(self):
         return self.resourceDirectory.__parent__.__parent__.__name__
 
     @zproperty.Lazy
     def baseUrl(self):
-        return '{0}/++{1}++{2}'.format(
-            self.portalUrl,
-            self.resourceType,
-            self.resourceDirectory.__name__
+        return "{}/++{}++{}".format(
+            self.portalUrl, self.resourceType, self.resourceDirectory.__name__
         )
 
     @zproperty.Lazy
     def fileConnector(self):
-        return '{0}/@@{1}'.format(self.baseUrl, self.__name__,)
+        return f"{self.baseUrl}/@@{self.__name__}"
 
     @zproperty.Lazy
     def filemanagerConfiguration(self):
         return """\
 var FILE_ROOT = '/';
-var IMAGES_EXT = {0};
-var CAPABILITIES = {1};
-var FILE_CONNECTOR = '{2}';
-var BASE_URL = '{3}';
+var IMAGES_EXT = {};
+var CAPABILITIES = {};
+var FILE_CONNECTOR = '{}';
+var BASE_URL = '{}';
 """.format(
             repr(self.imageExtensions),
             repr(self.capabilities),
             self.fileConnector,
             self.baseUrl,
         )
 
     def normalizePath(self, path):
-        if path.startswith('/'):
+        if path.startswith("/"):
             path = path[1:]
-        if path.endswith('/'):
+        if path.endswith("/"):
             path = path[:-1]
         return path
 
     def normalizeReturnPath(self, path):
-        if path.endswith('/'):
+        if path.endswith("/"):
             path = path[:-1]
-        if not path.startswith('/'):
-            path = '/' + path
+        if not path.startswith("/"):
+            path = "/" + path
         return path
 
     def parentPath(self, path):
-        return '/'.join(path.split('/')[:-1])
+        return "/".join(path.split("/")[:-1])
 
     # AJAX responses
 
     def getFolder(self, path, getSizes=False):
         """Returns a dict of file and folder objects representing the
         contents of the given directory (indicated by a "path" parameter). The
         values are dicts as returned by getInfo().
@@ -767,501 +778,472 @@
 
         Optionally a "type" parameter can be specified to restrict returned
         files (depending on the connector). If a "type" parameter is given for
         the HTML document, the same parameter value is reused and passed
         to getFolder(). This can be used for example to only show image files
         in a file system tree.
         """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
         folders = []
         files = []
 
         path = self.normalizePath(path)
         folder = self.getObject(path)
 
         for name in folder.listDirectory():
             if IResourceDirectory.providedBy(folder[name]):
-                folders.append(self.getInfo(
-                    path='{0}/{1}/'.format(path, name), getSize=getSizes))
+                folders.append(self.getInfo(path=f"{path}/{name}/", getSize=getSizes))
             else:
-                files.append(self.getInfo(
-                    path='{0}/{1}'.format(path, name), getSize=getSizes))
+                files.append(self.getInfo(path=f"{path}/{name}", getSize=getSizes))
         return folders + files
 
     def getInfo(self, path, getSize=False):
         """Returns information about a single file. Requests
         with mode "getinfo" will include an additional parameter, "path",
         indicating which file to inspect. A boolean parameter "getsize"
         indicates whether the dimensions of the file (if an image) should be
         returned.
         """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
         path = self.normalizePath(path)
         obj = self.getObject(path)
 
         filename = obj.__name__
-        error = ''
+        error = ""
         errorCode = 0
 
         properties = {
-            'dateModified': None,
+            "dateModified": None,
         }
 
         if isinstance(obj, File):
-            properties['dateModified'] = DateTime(obj._p_mtime).strftime('%c')
+            properties["dateModified"] = DateTime(obj._p_mtime).strftime("%c")
             size = obj.get_size() / 1024
             if size < 1024:
-                size_specifier = u'kb'
+                size_specifier = "kb"
             else:
-                size_specifier = u'mb'
+                size_specifier = "mb"
                 size = size / 1024
-            properties['size'] = '{0}{1}'.format(
+            properties["size"] = "{}{}".format(
                 size,
-                translate(_(u'filemanager_{0}'.format(size_specifier),
-                            default=size_specifier), context=self.request)
+                translate(
+                    _(f"filemanager_{size_specifier}", default=size_specifier),
+                    context=self.request,
+                ),
             )
 
-        fileType = 'txt'
+        fileType = "txt"
 
         siteUrl = self.portalUrl
         resourceName = self.resourceDirectory.__name__
 
-        preview = '{0}/{1}/images/fileicons/default.png'.format(
-            siteUrl,
-            self.staticFiles
-        )
+        preview = f"{siteUrl}/{self.staticFiles}/images/fileicons/default.png"
 
         if IResourceDirectory.providedBy(obj):
-            preview = '{0}/{1}/images/fileicons/_Open.png'.format(
-                siteUrl,
-                self.staticFiles
+            preview = "{}/{}/images/fileicons/_Open.png".format(
+                siteUrl, self.staticFiles
             )
-            fileType = 'dir'
-            path = path + '/'
+            fileType = "dir"
+            path = path + "/"
         else:
             fileType = self.getExtension(path, obj)
             if fileType in self.imageExtensions:
-                preview = '{0}/++{1}++{2}/{3}'.format(
-                    siteUrl,
-                    self.resourceType,
-                    resourceName,
-                    path
+                preview = "{}/++{}++{}/{}".format(
+                    siteUrl, self.resourceType, resourceName, path
                 )
             elif fileType in self.extensionsWithIcons:
-                preview = '{0}/{1}/images/fileicons/{2}.png'.format(
-                    siteUrl,
-                    self.staticFiles,
-                    fileType
+                preview = "{}/{}/images/fileicons/{}.png".format(
+                    siteUrl, self.staticFiles, fileType
                 )
 
         if isinstance(obj, Image):
-            properties['height'] = obj.height
-            properties['width'] = obj.width
+            properties["height"] = obj.height
+            properties["width"] = obj.width
 
         return {
-            'path': self.normalizeReturnPath(path),
-            'filename': filename,
-            'fileType': fileType,
-            'preview': preview,
-            'properties': properties,
-            'error': error,
-            'code': errorCode,
+            "path": self.normalizeReturnPath(path),
+            "filename": filename,
+            "fileType": fileType,
+            "preview": preview,
+            "properties": properties,
+            "error": error,
+            "code": errorCode,
         }
 
     def addFolder(self, path, name):
-        """Create a new directory on the server within the given path.
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            name = safe_encode(name, 'utf-8')
-
+        """Create a new directory on the server within the given path."""
         code = 0
-        error = ''
+        error = ""
 
         parentPath = self.normalizePath(path)
         parent = None
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if not validateFilename(name):
-                error = translate(_(u'filemanager_invalid_foldername',
-                                  default=u'Invalid folder name.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_invalid_foldername", default="Invalid folder name."),
+                    context=self.request,
+                )
                 code = 1
             elif name in parent:
-                error = translate(_(u'filemanager_error_folder_exists',
-                                  default=u'Folder already exists.'),
-                                  context=self.request)
+                error = translate(
+                    _(
+                        "filemanager_error_folder_exists",
+                        default="Folder already exists.",
+                    ),
+                    context=self.request,
+                )
                 code = 1
             else:
                 try:
                     parent.makeDirectory(name)
                 except UnicodeDecodeError:
                     error = translate(
                         _(
-                            u'filemanager_invalid_foldername',
-                            default=u'Invalid folder name.'
+                            "filemanager_invalid_foldername",
+                            default="Invalid folder name.",
                         ),
-                        context=self.request
+                        context=self.request,
                     )
                     code = 1
 
         return {
-            'parent': self.normalizeReturnPath(parentPath),
-            'name': name,
-            'error': error,
-            'code': code,
+            "parent": self.normalizeReturnPath(parentPath),
+            "name": name,
+            "error": error,
+            "code": code,
         }
 
     def add(self, path, newfile, replacepath=None):
         """Add the uploaded file to the specified path. Unlike
         the other methods, this method must return its JSON response wrapped in
         an HTML <textarea>, so the MIME type of the response is text/html
         instead of text/plain. The upload form in the File Manager passes the
         current path as a POST param along with the uploaded file. The response
         includes the path as well as the name used to store the file. The
         uploaded file's name should be safe to use as a path component in a
         URL, so URL-encoded at a minimum.
         """
-
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-        if six.PY2 and replacepath is not None:
-            replacepath = safe_encode(replacepath, 'utf-8')
-
         parentPath = self.normalizePath(path)
 
-        error = ''
+        error = ""
         code = 0
 
         name = newfile.filename
-        if six.PY2 and isinstance(name, six.text_type):
-            name = safe_encode(name, 'utf-8')
-
         if replacepath:
             newPath = replacepath
-            parentPath = '/'.join(replacepath.split('/')[:-1])
+            parentPath = "/".join(replacepath.split("/")[:-1])
         else:
-            newPath = '{0}/{1}'.format(parentPath, name,)
+            newPath = f"{parentPath}/{name}"
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if name in parent and not replacepath:
-                error = translate(_(u'filemanager_error_file_exists',
-                                  default=u'File already exists.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_error_file_exists", default="File already exists."),
+                    context=self.request,
+                )
                 code = 1
             else:
                 try:
                     self.resourceDirectory.writeFile(newPath, newfile)
                 except ValueError:
-                    error = translate(_(u'filemanager_error_file_invalid',
-                                      default=u'Could not read file.'),
-                                      context=self.request)
+                    error = translate(
+                        _(
+                            "filemanager_error_file_invalid",
+                            default="Could not read file.",
+                        ),
+                        context=self.request,
+                    )
                     code = 1
 
         return {
-            'parent': self.normalizeReturnPath(parentPath),
-            'path': self.normalizeReturnPath(path),
-            'name': name,
-            'error': error,
-            'code': code,
+            "parent": self.normalizeReturnPath(parentPath),
+            "path": self.normalizeReturnPath(path),
+            "name": name,
+            "error": error,
+            "code": code,
         }
 
     def addNew(self, path, name):
-        """Add a new empty file in the given directory
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            name = safe_encode(name, 'utf-8')
-
-        error = ''
+        """Add a new empty file in the given directory"""
+        error = ""
         code = 0
 
         parentPath = self.normalizePath(path)
-        newPath = '{0}/{1}'.format(parentPath, name,)
+        newPath = f"{parentPath}/{name}"
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if not validateFilename(name):
-                error = translate(_(u'filemanager_invalid_filename',
-                                  default=u'Invalid file name.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_invalid_filename", default="Invalid file name."),
+                    context=self.request,
+                )
                 code = 1
             elif name in parent:
-                error = translate(_(u'filemanager_error_file_exists',
-                                  default=u'File already exists.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_error_file_exists", default="File already exists."),
+                    context=self.request,
+                )
                 code = 1
             else:
-                self.resourceDirectory.writeFile(newPath, b'')
+                self.resourceDirectory.writeFile(newPath, b"")
 
         return {
-            'parent': self.normalizeReturnPath(parentPath),
-            'name': name,
-            'error': error,
-            'code': code,
+            "parent": self.normalizeReturnPath(parentPath),
+            "name": name,
+            "error": error,
+            "code": code,
         }
 
     def rename(self, path, newName):
-        """Rename the item at the given path to the new name
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            newName = safe_encode(newName, 'utf-8')
-
+        """Rename the item at the given path to the new name"""
         npath = self.normalizePath(path)
-        oldPath = newPath = '/'.join(npath.split('/')[:-1])
-        oldName = npath.split('/')[-1]
+        oldPath = newPath = "/".join(npath.split("/")[:-1])
+        oldName = npath.split("/")[-1]
 
         code = 0
-        error = ''
+        error = ""
 
         try:
             parent = self.getObject(oldPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             if newName != oldName:
                 if newName in parent:
                     error = translate(
-                        _(u'filemanager_error_file_exists',
-                          default=u'File already exists.'),
-                        context=self.request)
+                        _(
+                            "filemanager_error_file_exists",
+                            default="File already exists.",
+                        ),
+                        context=self.request,
+                    )
                     code = 1
                 else:
                     parent.rename(oldName, newName)
 
         return {
-            'oldParent': self.normalizeReturnPath(oldPath),
-            'oldName': oldName,
-            'newParent': self.normalizeReturnPath(newPath),
-            'newName': newName,
-            'error': error,
-            'code': code,
+            "oldParent": self.normalizeReturnPath(oldPath),
+            "oldName": oldName,
+            "newParent": self.normalizeReturnPath(newPath),
+            "newName": newName,
+            "error": error,
+            "code": code,
         }
 
     def delete(self, path):
-        """Delete the item at the given path.
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
+        """Delete the item at the given path."""
         npath = self.normalizePath(path)
-        parentPath = '/'.join(npath.split('/')[:-1])
-        name = npath.split('/')[-1]
+        parentPath = "/".join(npath.split("/")[:-1])
+        name = npath.split("/")[-1]
         code = 0
-        error = ''
+        error = ""
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
         else:
             try:
                 del parent[name]
             except KeyError:
-                error = translate(_(u'filemanager_error_file_not_found',
-                                  default=u'File not found.'),
-                                  context=self.request)
+                error = translate(
+                    _("filemanager_error_file_not_found", default="File not found."),
+                    context=self.request,
+                )
                 code = 1
 
         return {
-            'path': self.normalizeReturnPath(path),
-            'error': error,
-            'code': code,
+            "path": self.normalizeReturnPath(path),
+            "error": error,
+            "code": code,
         }
 
     def move(self, path, directory):
-        """Move the item at the given path to a new directory
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            directory = safe_encode(directory, 'utf-8')
-
+        """Move the item at the given path to a new directory"""
         npath = self.normalizePath(path)
         newParentPath = self.normalizePath(directory)
 
         parentPath = self.parentPath(npath)
-        filename = npath.split('/')[-1]
+        filename = npath.split("/")[-1]
 
         code = 0
-        error = ''
-        newCanonicalPath = '{0}/{1}'.format(newParentPath, filename)
+        error = ""
+        newCanonicalPath = f"{newParentPath}/{filename}"
 
         try:
             parent = self.getObject(parentPath)
         except KeyError:
-            error = translate(_(u'filemanager_invalid_parent',
-                              default=u'Parent folder not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_invalid_parent", default="Parent folder not found."),
+                context=self.request,
+            )
             code = 1
             return {
-                'code': code,
-                'error': error,
-                'newPath': self.normalizeReturnPath(newCanonicalPath),
+                "code": code,
+                "error": error,
+                "newPath": self.normalizeReturnPath(newCanonicalPath),
             }
 
         try:
             target = self.getObject(newParentPath)
         except KeyError:
-            error = translate(_(u'filemanager_error_folder_exists',
-                              default=u'Destination folder not found.'),
-                              context=self.request)
+            error = translate(
+                _(
+                    "filemanager_error_folder_exists",
+                    default="Destination folder not found.",
+                ),
+                context=self.request,
+            )
             code = 1
             return {
-                'code': code,
-                'error': error,
-                'newPath': self.normalizeReturnPath(newCanonicalPath),
+                "code": code,
+                "error": error,
+                "newPath": self.normalizeReturnPath(newCanonicalPath),
             }
 
         if filename not in parent:
-            error = translate(_(u'filemanager_error_file_not_found',
-                              default=u'File not found.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_error_file_not_found", default="File not found."),
+                context=self.request,
+            )
             code = 1
         elif filename in target:
-            error = translate(_(u'filemanager_error_file_exists',
-                              default=u'File already exists.'),
-                              context=self.request)
+            error = translate(
+                _("filemanager_error_file_exists", default="File already exists."),
+                context=self.request,
+            )
             code = 1
         else:
             obj = parent[filename]
             del parent[filename]
             target[filename] = obj
 
         return {
-            'code': code,
-            'error': error,
-            'newPath': self.normalizeReturnPath(newCanonicalPath),
+            "code": code,
+            "error": error,
+            "newPath": self.normalizeReturnPath(newCanonicalPath),
         }
 
     def download(self, path):
-        """Serve the requested file to the user
-        """
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
+        """Serve the requested file to the user"""
         npath = self.normalizePath(path)
-        parentPath = '/'.join(npath.split('/')[:-1])
-        name = npath.split('/')[-1]
+        parentPath = "/".join(npath.split("/")[:-1])
+        name = npath.split("/")[-1]
 
         parent = self.getObject(parentPath)
 
-        self.request.response.setHeader('Content-Type',
-                                        'application/octet-stream')
+        self.request.response.setHeader("Content-Type", "application/octet-stream")
         self.request.response.setHeader(
-            'Content-Disposition',
-            'attachment; filename="{0}"'.format(name)
+            "Content-Disposition", f'attachment; filename="{name}"'
         )
 
         # TODO: Use streams here if we can
         return parent.readFile(name)
 
     # Helpers
     def getObject(self, path):
         path = self.normalizePath(path)
         if not path:
             return self.resourceDirectory
         try:
             return self.resourceDirectory[path]
-        except (KeyError, NotFound,):
+        except (
+            KeyError,
+            NotFound,
+        ):
             raise KeyError(path)
 
     def getExtension(self, path, obj):
         basename, ext = os.path.splitext(path)
         ext = ext[1:].lower()
 
         ct = obj.getContentType()
         if ct:
             # take content type of the file over extension if available
-            if '/' in ct:
-                _ext = ct.split('/')[1].lower()
+            if "/" in ct:
+                _ext = ct.split("/")[1].lower()
             if _ext in self.extensionsWithIcons:
                 return _ext
         return ext
 
     # Methods that are their own views
     def getFile(self, path):
         self.setup()
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-
         path = self.normalizePath(path)
         file = self.context.context.unrestrictedTraverse(path)
         ext = self.getExtension(path, file)
-        result = {'ext': ext}
+        result = {"ext": ext}
         if ext not in self.imageExtensions:
-            result['contents'] = str(file.data)
+            result["contents"] = str(file.data)
         else:
             info = self.getInfo(path)
-            result['info'] = self.previewTemplate(info=info)
+            result["info"] = self.previewTemplate(info=info)
 
-        self.request.response.setHeader('Content-Type', 'application/json')
+        self.request.response.setHeader("Content-Type", "application/json")
         return json.dumps(result)
 
     def saveFile(self, path, value):
-        path = self.request.form.get('path', path)
-        value = self.request.form.get('value', value)
-        if six.PY2:
-            path = safe_encode(path, 'utf-8')
-            value = safe_encode(value, 'utf-8')
-        path = path.lstrip('/')
-        value = value.replace('\r\n', '\n')
+        path = self.request.form.get("path", path)
+        value = self.request.form.get("value", value)
+        path = path.lstrip("/")
+        value = value.replace("\r\n", "\n")
         self.context.writeFile(path, value)
-        return ' '  # Zope no likey empty responses
+        return " "  # Zope does not like empty responses
 
     def filetree(self):
+        foldersOnly = bool(self.request.get("foldersOnly", False))
 
-        foldersOnly = bool(self.request.get('foldersOnly', False))
-
-        def getFolder(root, relpath=''):
+        def getFolder(root, relpath=""):
             result = []
             for name in root.listDirectory():
-                path = '{0}/{1}'.format(relpath, name)
+                path = f"{relpath}/{name}"
                 if IResourceDirectory.providedBy(root[name]):
-                    item = {
-                        'title': name,
-                        'key': path,
-                        'isFolder': True
-                    }
-                    item['children'] = getFolder(root[name], path)
+                    item = {"title": name, "key": path, "isFolder": True}
+                    item["children"] = getFolder(root[name], path)
                     result.append(item)
                 elif not foldersOnly:
-                    item = {'title': name, 'key': path}
+                    item = {"title": name, "key": path}
                     result.append(item)
             return result
-        return json.dumps([{
-            'title': '/',
-            'key': '/',
-            'isFolder': True,
-            'expand': True,
-            'children': getFolder(self.context)
-        }])
+
+        return json.dumps(
+            [
+                {
+                    "title": "/",
+                    "key": "/",
+                    "isFolder": True,
+                    "expand": True,
+                    "children": getFolder(self.context),
+                }
+            ]
+        )
```

### Comparing `plone.resourceeditor-3.0.4/plone/resourceeditor/configure.zcml` & `plone.resourceeditor-4.0.0/plone/resourceeditor/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-    <include package="plone.staticresources" />
+  <include package="plone.staticresources" />
 
-    <permission
-        id="plone.resourceeditor.ManageSources"
-        title="plone.resourceeditor: Manage Sources"
-        />
-
-    <browser:page
-        name="plone.resourceeditor.filemanager-actions"
-        for="plone.resource.interfaces.IResourceDirectory"
-        class=".browser.FileManagerActions"
-        permission="plone.resourceeditor.ManageSources"
-        />
-
-    <browser:page
-        name="plone.resourceeditor.filemanager"
-        for="plone.resource.interfaces.IResourceDirectory"
-        class=".browser.FileManager"
-        template="editor.pt"
-        permission="plone.resourceeditor.ManageSources"
-        />
-
-    <browser:page
-        name="plone.resourceeditor.getfile"
-        for="plone.resource.interfaces.IResourceDirectory"
-        class=".browser.FileManager"
-        attribute="getFile"
-        permission="plone.resourceeditor.ManageSources"
-        />
-
-    <browser:page
-        name="plone.resourceeditor.savefile"
-        for="plone.resource.interfaces.IResourceDirectory"
-        class=".browser.FileManager"
-        attribute="saveFile"
-        permission="plone.resourceeditor.ManageSources"
-        />
-
-    <browser:page
-        name="plone.resourceeditor.filetree"
-        for="plone.resource.interfaces.IResourceDirectory"
-        class=".browser.FileManager"
-        attribute="filetree"
-        permission="plone.resourceeditor.ManageSources"
-        />
+  <permission
+      id="plone.resourceeditor.ManageSources"
+      title="plone.resourceeditor: Manage Sources"
+      />
+
+  <browser:page
+      name="plone.resourceeditor.filemanager-actions"
+      for="plone.resource.interfaces.IResourceDirectory"
+      class=".browser.FileManagerActions"
+      permission="plone.resourceeditor.ManageSources"
+      />
+
+  <browser:page
+      name="plone.resourceeditor.filemanager"
+      for="plone.resource.interfaces.IResourceDirectory"
+      class=".browser.FileManager"
+      template="editor.pt"
+      permission="plone.resourceeditor.ManageSources"
+      />
+
+  <browser:page
+      name="plone.resourceeditor.getfile"
+      for="plone.resource.interfaces.IResourceDirectory"
+      class=".browser.FileManager"
+      attribute="getFile"
+      permission="plone.resourceeditor.ManageSources"
+      />
+
+  <browser:page
+      name="plone.resourceeditor.savefile"
+      for="plone.resource.interfaces.IResourceDirectory"
+      class=".browser.FileManager"
+      attribute="saveFile"
+      permission="plone.resourceeditor.ManageSources"
+      />
+
+  <browser:page
+      name="plone.resourceeditor.filetree"
+      for="plone.resource.interfaces.IResourceDirectory"
+      class=".browser.FileManager"
+      attribute="filetree"
+      permission="plone.resourceeditor.ManageSources"
+      />
 
 </configure>
```

### Comparing `plone.resourceeditor-3.0.4/plone/resourceeditor/editor.pt` & `plone.resourceeditor-4.0.0/plone/resourceeditor/editor.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-<div xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
-      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone">
-
-    <metal:block define-macro="resources">
-
-        <metal:block define-macro="dependency-css">
-            <link rel="stylesheet" type="text/css"
-                tal:attributes="href string:${portal_url}/++plone++static/filemanager-compiled.css" />
-        </metal:block>
-
-        <metal:block define-macro="filemanager-scripts">
-            <script type="text/javascript" tal:attributes="src string:${portal_url}/++plone++static/filemanager-compiled.min.js"></script>
-        </metal:block>
+<div xmlns="http://www.w3.org/1999/xhtml"
+     xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+     xmlns:metal="http://xml.zope.org/namespaces/metal"
+     xmlns:tal="http://xml.zope.org/namespaces/tal"
+     lang="en"
+     xml:lang="en"
+     i18n:domain="plone"
+>
+
+  <metal:block define-macro="resources">
+
+    <metal:block define-macro="dependency-css">
+      <link rel="stylesheet"
+            type="text/css"
+            tal:attributes="
+              href string:${portal_url}/++plone++static/filemanager-compiled.css;
+            "
+      />
     </metal:block>
 
-    <metal:block define-macro="filemanager"
-        tal:define="authenticator context/@@authenticator/authenticator | nothing">
+    <metal:block define-macro="filemanager-scripts">
+      <script type="text/javascript"
+              tal:attributes="
+                src string:${portal_url}/++plone++static/filemanager-compiled.min.js;
+              "
+      ></script>
+    </metal:block>
+  </metal:block>
 
-        <input tal:replace="structure authenticator" />
-        <div class="pat-filemanager"
-            tal:attributes="data-pat-filemanager view/pattern_options">
-        </div>
+  <metal:block define-macro="filemanager"
+               tal:define="
+                 authenticator context/@@authenticator/authenticator | nothing;
+               "
+  >
+
+    <input tal:replace="structure authenticator" />
+    <div class="pat-filemanager"
+         tal:attributes="
+           data-pat-filemanager view/pattern_options;
+         "
+    >
+    </div>
 
-    </metal:block>
+  </metal:block>
 </div>
```

### Comparing `plone.resourceeditor-3.0.4/plone/resourceeditor/preview.pt` & `plone.resourceeditor-4.0.0/plone/resourceeditor/preview.pt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 
-<div xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-     xmlns:tal="http://xml.zope.org/namespaces/tal"
-     xmlns:metal="http://xml.zope.org/namespaces/metal"
+<div xmlns="http://www.w3.org/1999/xhtml"
      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-     class="info" tal:define="info options/info;
-                              props info/properties;">
-    <img src="" tal:attributes="src info/preview" tal:condition="exists:info/preview" />
-    <p class="discreet details">
-        <b i18n:translate="file_preview_date_modified">Date Modified</b>: <span tal:replace="props/dateModified" />
-            <span tal:condition="not:props/dateModified">n/a</span>
-        <br/>
-        <b i18n:translate="file_preview_size">Size</b>: <span tal:condition="exists:props/size" tal:replace="props/size" />
-            <span tal:condition="not:exists:props/size">n/a</span>
-    </p>
+     xmlns:metal="http://xml.zope.org/namespaces/metal"
+     xmlns:tal="http://xml.zope.org/namespaces/tal"
+     class="info"
+     xml:lang="en"
+     tal:define="
+       info options/info;
+       props info/properties;
+     "
+>
+  <img src=""
+       tal:condition="exists:info/preview"
+       tal:attributes="
+         src info/preview;
+       "
+  />
+  <p class="discreet details">
+    <b i18n:translate="file_preview_date_modified">Date Modified</b>:
+    <span tal:replace="props/dateModified"></span>
+    <span tal:condition="not:props/dateModified">n/a</span>
+    <br />
+    <b i18n:translate="file_preview_size">Size</b>:
+    <span tal:condition="exists:props/size"
+          tal:replace="props/size"
+    ></span>
+    <span tal:condition="not:exists:props/size">n/a</span>
+  </p>
 </div>
```

### Comparing `plone.resourceeditor-3.0.4/plone/resourceeditor/testing.py` & `plone.resourceeditor-4.0.0/plone/resourceeditor/testing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import applyProfile
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 
 
 class PloneResourceEditor(PloneSandboxLayer):
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load ZCML
         import plone.resourceeditor
+
         self.loadZCML(
-            'configure.zcml',
-            package=plone.resourceeditor,
-            context=configurationContext
+            "configure.zcml", package=plone.resourceeditor, context=configurationContext
         )
 
     def setUpPloneSite(self, portal):
         # install plone.resource
-        applyProfile(portal, 'plone.resource:default')
+        applyProfile(portal, "plone.resource:default")
 
 
 PLONE_RESOURCE_EDITOR_FIXTURE = PloneResourceEditor()
 PLONE_RESOURCE_EDITOR_INTEGRATION_TESTING = IntegrationTesting(
-    bases=(PLONE_RESOURCE_EDITOR_FIXTURE, ),
-    name='plone.resourceeditor:Integration',
+    bases=(PLONE_RESOURCE_EDITOR_FIXTURE,),
+    name="plone.resourceeditor:Integration",
 )
```

### Comparing `plone.resourceeditor-3.0.4/plone/resourceeditor/tests/test_file_manager.py` & `plone.resourceeditor-4.0.0/plone/resourceeditor/tests/test_file_manager_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,395 +1,368 @@
-# -*- coding: utf-8 -*-
-from plone.resourceeditor.testing import PLONE_RESOURCE_EDITOR_INTEGRATION_TESTING  # noqa
+from plone.resourceeditor.testing import PLONE_RESOURCE_EDITOR_INTEGRATION_TESTING
 
-import six
+import json
 import unittest
 
 
 class TestResourceEditorOperations(unittest.TestCase):
-
     layer = PLONE_RESOURCE_EDITOR_INTEGRATION_TESTING
 
-    def _make_directory(self, resourcetype='theme', resourcename='mytheme'):
+    def _make_directory(self, resourcetype="theme", resourcename="mytheme"):
         from plone.resource.interfaces import IResourceDirectory
         from zope.component import getUtility
 
-        resources = getUtility(IResourceDirectory, name='persistent')
+        resources = getUtility(IResourceDirectory, name="persistent")
         resources.makeDirectory(resourcetype)
         resources[resourcetype].makeDirectory(resourcename)
 
         return resources[resourcetype][resourcename]
 
     def test_getinfo(self):
-        from plone.resourceeditor.browser import FileManager
-        r = self._make_directory()
+        from plone.resourceeditor.browser import FileManagerActions
 
-        r.writeFile('test.txt', b'A text file')
+        r = self._make_directory()
 
-        view = FileManager(r, self.layer['request'])
-        info = view.getInfo('/test.txt')
+        r.writeFile("test.txt", b"A text file")
+        view = FileManagerActions(r, self.layer["request"])
+        info = view.getInfo(r["test.txt"])
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['fileType'], 'txt')
-        self.assertEqual(info['filename'], 'test.txt')
-        self.assertEqual(info['path'], '/test.txt')
+        self.assertEqual(info["fileType"], "txt")
+        self.assertEqual(info["filename"], "test.txt")
+        self.assertEqual(info["path"], "/")
 
     def test_getfolder(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
 
-        r.makeDirectory('alpha')
-        r['alpha'].writeFile('beta.txt', b'Beta')
-        r['alpha'].makeDirectory('delta')
-        r['alpha']['delta'].writeFile('gamma.css', b'body')
+        r.makeDirectory("alpha")
+        r["alpha"].writeFile("beta.txt", b"Beta")
+        r["alpha"].makeDirectory("delta")
+        r["alpha"]["delta"].writeFile("gamma.css", b"body")
 
-        view = FileManager(r, self.layer['request'])
-        info = view.getFolder('/alpha')
+        view = FileManagerActions(r, self.layer["request"])
+        info = view.getFolder("/alpha")
 
         self.assertEqual(len(info), 2)
-
-        self.assertEqual(info[0]['code'], 0)
-        self.assertEqual(info[0]['error'], '')
-        self.assertEqual(info[0]['fileType'], 'dir')
-        self.assertEqual(info[0]['filename'], 'delta')
-        self.assertEqual(info[0]['path'], '/alpha/delta')
-
-        self.assertEqual(info[1]['code'], 0)
-        self.assertEqual(info[1]['error'], '')
-        self.assertEqual(info[1]['fileType'], 'txt')
-        self.assertEqual(info[1]['filename'], 'beta.txt')
-        self.assertEqual(info[1]['path'], '/alpha/beta.txt')
+        self.assertEqual(info[0]["fileType"], "dir")
+        self.assertEqual(info[0]["filename"], "delta")
+        self.assertEqual(info[0]["path"], "/alpha/delta/")
+
+        self.assertEqual(info[1]["fileType"], "txt")
+        self.assertEqual(info[1]["filename"], "beta.txt")
+        self.assertEqual(info[1]["path"], "/alpha/beta.txt")
 
     def test_addfolder(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.addFolder('/', 'alpha')
+        info_str = view.addFolder("/", "alpha")
+        info = json.loads(info_str)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['parent'], '/')
-        self.assertEqual(info['name'], 'alpha')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["parent"], "/")
+        self.assertEqual(info["name"], "alpha")
 
-        info = view.addFolder('/alpha', 'beta')
+        info_str = view.addFolder("/alpha", "beta")
+        info = json.loads(info_str)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['parent'], '/alpha')
-        self.assertEqual(info['name'], 'beta')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["parent"], "/alpha")
+        self.assertEqual(info["name"], "beta")
 
     def test_addfolder_exists(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.makeDirectory('alpha')
+        r.makeDirectory("alpha")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.addFolder('/', 'alpha')
+        info_str = view.addFolder("/", "alpha")
+        info = json.loads(info_str)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-        self.assertEqual(info['parent'], '/')
-        self.assertEqual(info['name'], 'alpha')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
+        self.assertEqual(info["parent"], "/")
+        self.assertEqual(info["name"], "alpha")
 
     def test_addfolder_invalid_name(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.makeDirectory('alpha')
+        r.makeDirectory("alpha")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
         for char in '\\/:*?"<>':
-            info = view.addFolder('/', 'foo' + char)
+            info = view.addFolder("/", "foo" + char)
+            info = json.loads(info)
 
-            self.assertEqual(info['code'], 1)
-            self.assertNotEqual(info['error'], '')
-            self.assertEqual(info['parent'], '/')
-            self.assertEqual(info['name'], 'foo' + char)
+            self.assertEqual(info["code"], 1)
+            self.assertNotEqual(info["error"], "")
+            self.assertEqual(info["parent"], "/")
+            self.assertEqual(info["name"], "foo" + char)
 
     def test_addfolder_invalid_parent(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.addFolder('/alpha', 'beta')
+        info = view.addFolder("/alpha", "beta")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-        self.assertEqual(info['parent'], '/alpha')
-        self.assertEqual(info['name'], 'beta')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
+        self.assertEqual(info["parent"], "/alpha")
+        self.assertEqual(info["name"], "beta")
 
     def test_add(self):
-        from plone.resourceeditor.browser import FileManager
-        from six import BytesIO
-        r = self._make_directory()
+        from plone.resourceeditor.browser import FileManagerActions
 
-        view = FileManager(r, self.layer['request'])
-
-        d = BytesIO(b'foo')
-        d.filename = 'test.txt'
-        info = view.add('/', d)
-
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['name'], 'test.txt')
-        self.assertEqual(info['path'], '/')
-        self.assertEqual(info['parent'], '/')
-
-    def test_add_subfolder(self):
-        from plone.resourceeditor.browser import FileManager
-        from six import BytesIO
         r = self._make_directory()
-        r.makeDirectory('alpha')
-
-        view = FileManager(r, self.layer['request'])
 
-        d = BytesIO(b'foo')
-        d.filename = 'test.txt'
-
-        info = view.add('/alpha', d)
-
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['name'], 'test.txt')
-        self.assertEqual(info['path'], '/alpha')
-        self.assertEqual(info['parent'], '/alpha')
-
-    def test_add_exists(self):
-        from plone.resourceeditor.browser import FileManager
-        from six import BytesIO
-        r = self._make_directory()
-        r.writeFile('test.txt', b'boo')
+        view = FileManagerActions(r, self.layer["request"])
 
-        view = FileManager(r, self.layer['request'])
+        d = "test.txt"
 
-        d = BytesIO(b'foo')
-        d.filename = 'test.txt'
+        info = view.addFile("/", d)
+        info = json.loads(info)
 
-        info = view.add('/', d)
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["name"], "test.txt")
+        self.assertEqual(info["path"], "/")
+        self.assertEqual(info["parent"], "/")
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-
-        self.assertEqual(r.readFile('test.txt'), b'boo')
+    def test_add_subfolder(self):
+        from plone.resourceeditor.browser import FileManagerActions
 
-    def test_add_replace(self):
-        from plone.resourceeditor.browser import FileManager
-        from six import BytesIO
         r = self._make_directory()
-        r.writeFile('test.txt', b'boo')
+        r.makeDirectory("alpha")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        d = BytesIO(b'foo')
-        d.filename = 'test.txt'
+        d = "test.txt"
 
-        info = view.add('/', d, '/test.txt')
+        info = view.addFile("/alpha", d)
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['name'], 'test.txt')
-        self.assertEqual(info['path'], '/')
-        self.assertEqual(info['parent'], '/')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["name"], "test.txt")
+        self.assertEqual(info["path"], "/alpha")
+        self.assertEqual(info["parent"], "/alpha")
 
-        self.assertEqual(r.readFile('test.txt'), b'foo')
+    def test_add_exists(self):
+        from plone.resourceeditor.browser import FileManagerActions
 
-    def test_addnew(self):
-        from plone.resourceeditor.browser import FileManager
         r = self._make_directory()
+        r.writeFile("test.txt", b"boo")
 
-        view = FileManager(r, self.layer['request'])
-
-        info = view.addNew('/', 'test.txt')
-
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['name'], 'test.txt')
-        self.assertEqual(info['parent'], '/')
+        view = FileManagerActions(r, self.layer["request"])
 
-        self.assertEqual(r.readFile('test.txt'), b'')
+        d = "test.txt"
 
-    def test_addnew_exists(self):
-        from plone.resourceeditor.browser import FileManager
-        r = self._make_directory()
-        r.writeFile('test.txt', b'foo')
-
-        view = FileManager(r, self.layer['request'])
-
-        info = view.addNew('/', 'test.txt')
+        info = view.addFile("/", d)
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
 
-        self.assertEqual(r.readFile('test.txt'), b'foo')
+        self.assertEqual(r.readFile("test.txt"), b"boo")
 
     def test_addnew_invalidname(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
         for char in '\\/:*?"<>':
-            info = view.addNew('/', 'foo' + char)
-            self.assertEqual(info['code'], 1)
-            self.assertNotEqual(info['error'], '')
+            info = view.addFile("/", "foo" + char)
+            info = json.loads(info)
+            self.assertEqual(info["code"], 1)
+            self.assertNotEqual(info["error"], "")
 
     def test_rename(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.writeFile('test.txt', b'foo')
+        r.writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.rename('/test.txt', 'foo.txt')
+        info = view.renameFile("/test.txt", "foo.txt")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['oldName'], 'test.txt')
-        self.assertEqual(info['newName'], 'foo.txt')
-        self.assertEqual(info['oldParent'], '/')
-        self.assertEqual(info['newParent'], '/')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["oldName"], "test.txt")
+        self.assertEqual(info["newName"], "foo.txt")
+        self.assertEqual(info["oldParent"], "/")
+        self.assertEqual(info["newParent"], "/")
 
-        self.assertEqual(r.readFile('foo.txt'), b'foo')
+        self.assertEqual(r.readFile("foo.txt"), b"foo")
 
     def test_rename_subfolder(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.makeDirectory('alpha')
-        r['alpha'].writeFile('test.txt', b'foo')
+        r.makeDirectory("alpha")
+        r["alpha"].writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.rename('/alpha/test.txt', 'foo.txt')
+        info = view.renameFile("/alpha/test.txt", "foo.txt")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['oldName'], 'test.txt')
-        self.assertEqual(info['newName'], 'foo.txt')
-        self.assertEqual(info['oldParent'], '/alpha')
-        self.assertEqual(info['newParent'], '/alpha')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["oldName"], "test.txt")
+        self.assertEqual(info["newName"], "foo.txt")
+        self.assertEqual(info["oldParent"], "/alpha")
+        self.assertEqual(info["newParent"], "/alpha")
 
-        self.assertEqual(r['alpha'].readFile('foo.txt'), b'foo')
+        self.assertEqual(r["alpha"].readFile("foo.txt"), b"foo")
 
     def test_rename_exists(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.writeFile('test.txt', b'foo')
-        r.writeFile('foo.txt', b'bar')
+        r.writeFile("test.txt", b"foo")
+        r.writeFile("foo.txt", b"bar")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.rename('/test.txt', 'foo.txt')
+        info = view.renameFile("/test.txt", "foo.txt")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-        self.assertEqual(info['oldName'], 'test.txt')
-        self.assertEqual(info['newName'], 'foo.txt')
-        self.assertEqual(info['oldParent'], '/')
-        self.assertEqual(info['newParent'], '/')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
+        self.assertEqual(info["oldName"], "test.txt")
+        self.assertEqual(info["newName"], "foo.txt")
+        self.assertEqual(info["oldParent"], "/")
+        self.assertEqual(info["newParent"], "/")
 
-        self.assertEqual(r.readFile('foo.txt'), b'bar')
+        self.assertEqual(r.readFile("foo.txt"), b"bar")
 
     def test_delete(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.writeFile('test.txt', b'foo')
+        r.writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.delete('/test.txt')
+        info = view.delete("/test.txt")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['path'], '/test.txt')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["path"], "/test.txt")
 
-        self.assertFalse('test.txt' in r)
+        self.assertFalse("test.txt" in r)
 
     def test_delete_subfolder(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.makeDirectory('alpha')
-        r['alpha'].writeFile('test.txt', b'foo')
+        r.makeDirectory("alpha")
+        r["alpha"].writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.delete('/alpha/test.txt')
+        info = view.delete("/alpha/test.txt")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['path'], '/alpha/test.txt')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["path"], "/alpha/test.txt")
 
-        self.assertFalse('test.txt' in r['alpha'])
+        self.assertFalse("test.txt" in r["alpha"])
 
     def test_delete_notfound(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.delete('/test.txt')
+        info = view.delete("/test.txt")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-        self.assertEqual(info['path'], '/test.txt')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
+        self.assertEqual(info["path"], "/test.txt")
 
     def test_move(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.makeDirectory('alpha')
-        r.writeFile('test.txt', b'foo')
+        r.makeDirectory("alpha")
+        r.writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.move('/test.txt', '/alpha')
+        info = view.move("/test.txt", "/alpha")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 0)
-        self.assertEqual(info['error'], '')
-        self.assertEqual(info['newPath'], '/alpha/test.txt')
+        self.assertEqual(info["code"], 0)
+        self.assertEqual(info["error"], "")
+        self.assertEqual(info["newPath"], "/alpha/test.txt")
 
-        self.assertFalse('test.txt' in r)
-        self.assertEqual(b'foo', r['alpha'].readFile('test.txt'))
+        self.assertFalse("test.txt" in r)
+        self.assertEqual(b"foo", r["alpha"].readFile("test.txt"))
 
     def test_move_exists(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.makeDirectory('alpha')
-        r['alpha'].writeFile('test.txt', b'bar')
-        r.writeFile('test.txt', b'foo')
+        r.makeDirectory("alpha")
+        r["alpha"].writeFile("test.txt", b"bar")
+        r.writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.move('/test.txt', '/alpha')
+        info = view.move("/test.txt", "/alpha")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-        self.assertEqual(info['newPath'], '/alpha/test.txt')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
+        self.assertEqual(info["newPath"], "/alpha/test.txt")
 
-        self.assertTrue('test.txt' in r)
-        self.assertEqual(b'bar', r['alpha'].readFile('test.txt'))
+        self.assertTrue("test.txt" in r)
+        self.assertEqual(b"bar", r["alpha"].readFile("test.txt"))
 
     def test_move_invalid_parent(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.writeFile('test.txt', b'foo')
+        r.writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
+        view = FileManagerActions(r, self.layer["request"])
 
-        info = view.move('/test.txt', '/alpha')
+        info = view.move("/test.txt", "/alpha")
+        info = json.loads(info)
 
-        self.assertEqual(info['code'], 1)
-        self.assertNotEqual(info['error'], '')
-        self.assertEqual(info['newPath'], '/alpha/test.txt')
+        self.assertEqual(info["code"], 1)
+        self.assertNotEqual(info["error"], "")
+        self.assertEqual(info["newPath"], "/alpha/test.txt")
 
-        self.assertTrue('test.txt' in r)
+        self.assertTrue("test.txt" in r)
 
     def test_download(self):
-        from plone.resourceeditor.browser import FileManager
+        from plone.resourceeditor.browser import FileManagerActions
+
         r = self._make_directory()
-        r.writeFile('test.txt', b'foo')
+        r.writeFile("test.txt", b"foo")
 
-        view = FileManager(r, self.layer['request'])
-        self.assertEqual(b'foo', view.download('/test.txt'))
+        view = FileManagerActions(r, self.layer["request"])
+        self.assertEqual(b"foo", view.download("/test.txt"))
```

### Comparing `plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/PKG-INFO` & `plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: plone.resourceeditor
-Version: 3.0.4
+Version: 4.0.0
 Summary: Integrates ACE editor into Plone
 Home-page: https://github.com/plone/plone.resourceeditor
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: ace resource editor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Introduction
 ============
 
 This package contains resources for integrating `ACE embeddable code editor <http://ace.ajax.org>`_ into Plone.
 It provides a file manager that can edit ``plone.resource`` resource directories in the ZODB.
@@ -54,14 +52,31 @@
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
+- Drop python 2.7 compatibility.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (2a4ba395)
+
+
 3.0.4 (2022-08-30)
 ------------------
 
 Bug fixes:
 
 
 - Fix unclosed file warnings
@@ -157,15 +172,15 @@
 ------------------
 
 Fixes:
 
 - Remove  unittest2 dependency
   [kakshay21]
 - Split the error message for the move API endpoint into two. One
-  is for the parent folder and the other is for the distination folder
+  is for the parent folder and the other is for the destination folder
   [b4oshany]
 - Fix Jenkins flake8 errors
 
 
 [b4oshany]: https://github.com/b4oshany
 
 2.0.5 (2016-03-31)
@@ -206,15 +221,15 @@
 - handle NotFound errors while generating file/folder listings
   [vangheem]
 
 
 2.0.2 (2015-09-08)
 ------------------
 
-- Added check to prevent overwritting folders when saving
+- Added check to prevent overwriting folders when saving
   [obct537]
 
 2.0.1 (2015-08-22)
 ------------------
 
 - Added ability to convert absolute to relative urls
   [obct537]
```

### Comparing `plone.resourceeditor-3.0.4/plone.resourceeditor.egg-info/SOURCES.txt` & `plone.resourceeditor-4.0.0/plone.resourceeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

