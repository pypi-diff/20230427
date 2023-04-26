# Comparing `tmp/plone.transformchain-2.0.2.tar.gz` & `tmp/plone.transformchain-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.transformchain-2.0.2.tar", last modified: Wed Apr 22 21:28:33 2020, max compression
+gzip compressed data, was "plone.transformchain-3.0.0.tar", last modified: Wed Apr 26 22:05:38 2023, max compression
```

## Comparing `plone.transformchain-2.0.2.tar` & `plone.transformchain-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     8132 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      149 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1260 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1768 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/
--rw-r--r--   0 maurits    (501) staff       (20)     3723 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3578 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/zpublisher.py
--rw-r--r--   0 maurits    (501) staff       (20)      626 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1059 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/events.py
--rw-r--r--   0 maurits    (501) staff       (20)       24 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2385 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/transformer.py
--rw-r--r--   0 maurits    (501) staff       (20)    21016 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/transformchain/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     8132 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      718 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)      122 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/plone.transformchain.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      102 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     3274 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2118 2020-04-22 21:28:33.000000 plone.transformchain-2.0.2/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:05:38.982015 plone.transformchain-3.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     2312 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     6565 2023-04-26 22:05:38.982120 plone.transformchain-3.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3274 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:05:38.977818 plone.transformchain-3.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1260 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/docs/INSTALL.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:05:38.978110 plone.transformchain-3.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:05:38.981810 plone.transformchain-3.0.0/plone/transformchain/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      450 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      995 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3488 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20058 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2065 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/transformer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3173 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone/transformchain/zpublisher.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 22:05:38.979926 plone.transformchain-3.0.0/plone.transformchain.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     6565 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      671 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       43 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/plone.transformchain.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2858 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 22:05:38.982537 plone.transformchain-3.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1564 2023-04-26 22:05:38.000000 plone.transformchain-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.transformchain-2.0.2/docs/INSTALL.txt` & `plone.transformchain-3.0.0/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.transformchain-2.0.2/setup.py` & `plone.transformchain-3.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '2.0.2'
+version = "3.0.0"
 
 setup(
-    name='plone.transformchain',
+    name="plone.transformchain",
     version=version,
-    description=("Hook into repoze.zope2 that allows third party packages "
-                 "to register a sequence of hooks that will be allowed to "
-                 "modify the response before it is returned to the browser"),
-    long_description=(open("README.rst").read() + "\n" +
-                      open("CHANGES.rst").read()),
+    description=(
+        "Hook into repoze.zope2 that allows third party packages "
+        "to register a sequence of hooks that will be allowed to "
+        "modify the response before it is returned to the browser"
+    ),
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     # Get more strings from
     # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.0",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    keywords='zope2 repoze transform',
-    author='Martin Aspeli',
-    author_email='optilude@gmail.com',
-    url='https://pypi.org/project/plone.transformchain',
-    license='BSD',
+    keywords="zope2 repoze transform",
+    author="Martin Aspeli",
+    author_email="optilude@gmail.com",
+    url="https://pypi.org/project/plone.transformchain",
+    license="BSD",
     packages=find_packages(),
-    namespace_packages=['plone'],
+    namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     extras_require={
-        'repoze': ['repoze.zope2'],
-        'test': 'plone.testing [zca]',
+        "test": "plone.testing [zca]",
     },
     install_requires=[
-        'setuptools',
-        'six',
-        'zope.interface',
-        'zope.component',
-        'zope.schema',
-        'Zope2>=2.13.23'
+        "setuptools",
+        "Zope",
     ],
     entry_points="""
     """,
 )
```

### Comparing `plone.transformchain-2.0.2/plone/transformchain/interfaces.py` & `plone.transformchain-3.0.0/plone/transformchain/interfaces.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-# -*- coding: utf-8 -*-
 from zope import schema
 from zope.interface import Attribute
 from zope.interface import Interface
 
 
-try:
-    from repoze.zope2.interfaces import ITransformer as IBaseTransformer
-except ImportError:
-    IBaseTransformer = Interface
-
-DISABLE_TRANSFORM_REQUEST_KEY = 'plone.transformchain.disable'
+DISABLE_TRANSFORM_REQUEST_KEY = "plone.transformchain.disable"
 
 
 class ITransform(Interface):
     """Register a named multi adapter from (published, request,) to
     this interface to change the response.
 
     ``published`` is the published object, i.e. the last thing being traversed
@@ -21,45 +15,45 @@
 
     ``request`` is the request type.
 
     To control the order of transforms, use the 'order' attribute. It may be
     positive or negative.
     """
 
-    order = schema.Int(title=u"Order")
+    order = schema.Int(title="Order")
 
     def transformUnicode(result, encoding):
         """Called to allow the transformer to modify the result if the result
-        is a six.text_type string.
+        is text string.
 
-        Return a new six.text_type string, encoded string or iterable.
+        Return a new text string, encoded string or iterable.
 
         Return None to indicate that the response should not be modified.
         """
 
     def transformBytes(result, encoding):
         """Called to allow the transformer to modify the result if the result
         is an encoded string.
 
-        Return a new six.text_type string, encoded string or iterable.
+        Return a new text string, encoded string or iterable.
 
         Return None to indicate that the response should not be modified.
         """
 
     def transformIterable(result, encoding):
         """Called to allow the transformer to modify the result if the result
         is an iterable of strings (as per the WSGI specification).
 
-        Return a new six.text_type string, encoded string or iterable.
+        Return a new text string, encoded string or iterable.
 
         Return None to indicate that the response should not be modified.
         """
 
 
-class ITransformer(IBaseTransformer):
+class ITransformer(Interface):
     """Low-level hook. This interface is defined in repoze.zope2, but since
     this package can be used with the classic ZPublisher as well, we redefine
     it here. You probably don't want to use this directly; you want to use
     ITransform instead.
     """
 
     def __call__(request, result, encoding):
@@ -70,49 +64,45 @@
 
         `result` is an iterable of byte strings that represents the response
         body. When unwound, its contents will match the response content type.
 
         `encoding` is the default encoding used.
 
         Return the new result iterable, or a string. If a string is returned,
-        the Content-Type header will be updated automatically. If a six.text_type
+        the Content-Type header will be updated automatically. If a text
         string is returned, it will be encoded with the current content
         encoding.
 
         Do not call `request.response.setBody()`. It will have no effect.
         """
 
 
 class IBaseTransformEvent(Interface):
     """Base class for transform events.
 
     Transform events are notified at different points in transformations.
     """
-    request = Attribute('The request being affected')
+
+    request = Attribute("The request being affected")
 
 
 class IBeforeTransformsEvent(IBaseTransformEvent):
-    """Notified before any transforms are started.
-    """
+    """Notified before any transforms are started."""
 
 
 class IAfterTransformsEvent(IBaseTransformEvent):
-    """Notified after all transforms are finished.
-    """
+    """Notified after all transforms are finished."""
 
 
 class IBaseSingleTransformEvent(IBaseTransformEvent):
-    """Base class for a single transformation notification.
-    """
+    """Base class for a single transformation notification."""
 
-    name = Attribute('the name of the transformation')
-    handler = Attribute('the transformation handler')
+    name = Attribute("the name of the transformation")
+    handler = Attribute("the transformation handler")
 
 
 class IBeforeSingleTransformEvent(IBaseSingleTransformEvent):
-    """Notified before a single Transformation is executed.
-    """
+    """Notified before a single Transformation is executed."""
 
 
 class IAfterSingleTransformEvent(IBaseSingleTransformEvent):
-    """Notified after a single Transformation is executed.
-    """
+    """Notified after a single Transformation is executed."""
```

### Comparing `plone.transformchain-2.0.2/plone/transformchain/zpublisher.py` & `plone.transformchain-3.0.0/plone/transformchain/zpublisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,103 @@
-# -*- coding: utf-8 -*-
 from plone.transformchain.interfaces import ITransformer
 from zope.component import adapter
 from zope.component import queryUtility
-from zope.interface import Interface
 from ZPublisher.HTTPResponse import default_encoding
+from ZPublisher.interfaces import IPubBeforeAbort
 from ZPublisher.interfaces import IPubBeforeCommit
 from ZPublisher.Iterators import IStreamIterator
 
 import re
-import six
 
 
-try:
-    from ZPublisher.interfaces import IPubBeforeAbort
-except ImportError:
-    # old Zope 2.12 or old ZPublisherBackport - this interface won't be
-    # used, most likely, so the effect is that error messages aren't styled.
-    class IPubBeforeAbort(Interface):
-        pass
-
 CHARSET_RE = re.compile(
-    r'(?:application|text)/[-+0-9a-z]+\s*;\s?charset=([-_0-9a-z]+)'
-    r'(?:(?:\s*;)|\Z)',
-    re.IGNORECASE
+    r"(?:application|text)/[-+0-9a-z]+\s*;\s?charset=([-_0-9a-z]+)" r"(?:(?:\s*;)|\Z)",
+    re.IGNORECASE,
 )
 
 
 def extractEncoding(response):
-    """Get the content encoding for the response body
-    """
+    """Get the content encoding for the response body"""
     encoding = default_encoding
-    ct = response.headers.get('content-type')
+    ct = response.headers.get("content-type")
     if ct:
         match = CHARSET_RE.match(ct)
         if match:
             encoding = match.group(1)
     return encoding
 
 
 def isEvilWebDAVRequest(request):
-    if request.get('WEBDAV_SOURCE_PORT', None):
+    if request.get("WEBDAV_SOURCE_PORT", None):
         return True
 
-    if request.get('REQUEST_METHOD', 'GET').upper() not in ('GET', 'POST',):
+    if request.get("REQUEST_METHOD", "GET").upper() not in (
+        "GET",
+        "POST",
+    ):
         return True
 
-    if request.get('PATH_INFO', '').endswith('manage_DAVget'):
+    if request.get("PATH_INFO", "").endswith("manage_DAVget"):
         return True
 
     return False
 
 
 def applyTransform(request, body=None):
-    """Apply any transforms by delegating to the ITransformer utility
-    """
+    """Apply any transforms by delegating to the ITransformer utility"""
 
     if isEvilWebDAVRequest(request):
         return None
 
     transformer = queryUtility(ITransformer)
     if transformer is not None:
         response = request.response
         encoding = extractEncoding(response)
 
         if body is None:
             body = response.getBody()
 
         result = body
-        if isinstance(result, six.binary_type):
+        if isinstance(result, bytes):
             result = [result]
-        elif isinstance(result, six.text_type):
+        elif isinstance(result, str):
             result = [result.encode(encoding)]
 
         transformed = transformer(request, result, encoding)
         if transformed is not None and transformed is not result:
             return transformed
 
     return None
 
 
 @adapter(IPubBeforeCommit)
 def applyTransformOnSuccess(event):
-    """Apply the transform after a successful request
-    """
+    """Apply the transform after a successful request"""
     transformed = applyTransform(event.request)
     if transformed is None:
         return
     response = event.request.response
 
     if IStreamIterator.providedBy(transformed):
         response.setBody(transformed)
     # setBody() can deal with byte and unicode strings (and will encode as
     # necessary)...
-    elif isinstance(transformed, six.string_types)\
-            or isinstance(transformed, six.binary_type):
+    elif isinstance(transformed, str) or isinstance(transformed, bytes):
         response.setBody(transformed)
     # ... but not with iterables
     else:
         transformed = map(
-            lambda it: it.decode('utf-8')
-            if isinstance(it, six.binary_type)
-            else it,
-            transformed
+            lambda it: it.decode("utf-8") if isinstance(it, bytes) else it, transformed
         )
-        response.setBody(''.join(transformed))
+        response.setBody("".join(transformed))
 
 
 @adapter(IPubBeforeAbort)
 def applyTransformOnFailure(event):
-    """Apply the transform to the error html output
-    """
+    """Apply the transform to the error html output"""
     if event.retry:
         return
     # response.status might still be 200 because
     # IPubBeforeAbort is notified before
     # ZPublisher.Publish.publish_module_standard
     # calls HTTPResponse.exception()
     # which actually updates the status
```

### Comparing `plone.transformchain-2.0.2/plone/transformchain/events.py` & `plone.transformchain-3.0.0/plone/transformchain/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-# -*- coding: utf-8 -*-
 from plone.transformchain.interfaces import IAfterSingleTransformEvent
 from plone.transformchain.interfaces import IAfterTransformsEvent
 from plone.transformchain.interfaces import IBeforeSingleTransformEvent
 from plone.transformchain.interfaces import IBeforeTransformsEvent
 from zope.interface import implementer
 
 
-class BaseTransformEvent(object):
-
+class BaseTransformEvent:
     def __init__(self, request):
         self.request = request
 
 
 class BaseSingleTransformEvent(BaseTransformEvent):
-
     def __init__(self, request, name, handler):
-        super(BaseSingleTransformEvent, self).__init__(request)
+        super().__init__(request)
         self.name = name
         self.handler = handler
 
 
 @implementer(IBeforeTransformsEvent)
 class BeforeTransforms(BaseTransformEvent):
     pass
```

### Comparing `plone.transformchain-2.0.2/plone/transformchain/tests.py` & `plone.transformchain-3.0.0/plone/transformchain/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.testing.zca import UNIT_TESTING
 from plone.transformchain.interfaces import ITransform
 from plone.transformchain.interfaces import ITransformer
 from plone.transformchain.transformer import Transformer
 from plone.transformchain.zpublisher import applyTransformOnSuccess
 from zope.component import adapter
 from zope.component import provideAdapter
@@ -10,81 +9,60 @@
 from zope.interface import alsoProvides
 from zope.interface import implementer
 from zope.interface import Interface
 from ZPublisher.HTTPResponse import default_encoding
 from ZPublisher.Iterators import filestream_iterator
 
 import os
-import pkg_resources
-import six
 import tempfile
 import unittest
 
 
-HAS_ZSERVER = True
-try:
-    dist = pkg_resources.get_distribution('ZServer')
-except pkg_resources.DistributionNotFound:
-    HAS_ZSERVER = False
-
-if HAS_ZSERVER:
-    from ZServer.FTPRequest import FTPRequest
-
-
-class FauxPubEvent(object):
-
+class FauxPubEvent:
     def __init__(self, request):
         self.request = request
 
 
 class IRequestMarker(Interface):
     pass
 
 
 class IPublishedMarker(Interface):
     pass
 
 
-class FauxResponse(object):
-
-    def __init__(self, body=''):
+class FauxResponse:
+    def __init__(self, body=""):
         self._body = body
         self.headers = {}
 
     def getBody(self):
         return self._body
 
     def setBody(self, body):
         self._body = body
 
 
 class FauxRequest(dict):
-
     def __init__(self, published, response=None):
         if response is None:
-            response = FauxResponse('<html/>')
+            response = FauxResponse("<html/>")
 
-        self['PUBLISHED'] = published
+        self["PUBLISHED"] = published
         self.response = response
         self.environ = {}
 
 
-if HAS_ZSERVER:
-    class FauxFTPRequest(FauxRequest, FTPRequest):
-        pass
-
-
-class FauxPublished(object):
+class FauxPublished:
     pass
 
 
 @implementer(ITransform)
 @adapter(Interface, Interface)
-class FauxTransformBase(object):
-
+class FauxTransformBase:
     order = 0
 
     def __init__(self, published, request):
         self.published = published
         self.request = request
 
     def transformBytes(self, result, encoding):
@@ -94,465 +72,423 @@
         return None
 
     def transformIterable(self, result, encoding):
         return None
 
 
 class TestTransformChain(unittest.TestCase):
-
     layer = UNIT_TESTING
 
     def setUp(self):
         self.t = Transformer()
 
     def test_simple(self):
-
         class Transform1(FauxTransformBase):
-
             def transformBytes(self, result, encoding):
-                return result + b' transformed'
+                return result + b" transformed"
 
             def transformUnicode(self, result, encoding):
-                return result + u' transformed'
+                return result + " transformed"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' transformed'
+                return "".join(result) + " transformed"
 
-        provideAdapter(Transform1, name=u'test.one')
+        provideAdapter(Transform1, name="test.one")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Blah']
-        encoding = 'utf-8'
+        result = ["Blah"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('Blah transformed', new_result)
+        self.assertEqual("Blah transformed", new_result)
 
     def test_off_switch(self):
-
         class Transform1(FauxTransformBase):
-
             order = 0
 
             def transformBytes(self, result, encoding):
-                return result + b' transformed'
+                return result + b" transformed"
 
             def transformUnicode(self, result, encoding):
-                return result + u' transformed'
+                return result + " transformed"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' transformed'
+                return "".join(result) + " transformed"
 
-        provideAdapter(Transform1, name=u'test.one')
+        provideAdapter(Transform1, name="test.one")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request.environ['plone.transformchain.disable'] = True
+        request.environ["plone.transformchain.disable"] = True
 
-        result = ['Blah']
-        encoding = 'utf-8'
+        result = ["Blah"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
         self.assertEqual(None, new_result)
 
-    @unittest.skipUnless(HAS_ZSERVER, 'ZServer is optional')
-    def test_ftp_request_not_transformed(self):
-        request = FauxFTPRequest(FauxPublished())
-        result = ['Blah']
-        new_result = self.t(request, result, 'utf8')
-        self.assertEqual(None, new_result)
-
     def test_transform_bytes(self):
-
         class Transform1(FauxTransformBase):
-
             def transformBytes(self, result, encoding):
-                return result + b' One'
+                return result + b" One"
 
-        provideAdapter(Transform1, name=u'test.one')
+        provideAdapter(Transform1, name="test.one")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = b'Blah'
-        encoding = 'utf-8'
+        result = b"Blah"
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual(b'Blah One', new_result)
+        self.assertEqual(b"Blah One", new_result)
 
     def test_transform_text(self):
-
         class Transform1(FauxTransformBase):
-
             def transformUnicode(self, result, encoding):
-                return result + u' One'
+                return result + " One"
 
-        provideAdapter(Transform1, name=u'test.one')
+        provideAdapter(Transform1, name="test.one")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = u'Blah'
-        encoding = 'utf-8'
+        result = "Blah"
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual(u'Blah One', new_result)
+        self.assertEqual("Blah One", new_result)
 
     def test_transform_iterable(self):
-
         class Transform1(FauxTransformBase):
-
             def transformIterable(self, result, encoding):
-                return result + [' One']
+                return result + [" One"]
 
-        provideAdapter(Transform1, name=u'test.one')
+        provideAdapter(Transform1, name="test.one")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Blah']
-        encoding = 'utf-8'
+        result = ["Blah"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual(['Blah', ' One'], new_result)
+        self.assertEqual(["Blah", " One"], new_result)
 
     def test_transform_mixed(self):
-
         class Transform1(FauxTransformBase):
-
             def transformIterable(self, result, encoding):
-                return u''.join(result) + u' One'
+                return "".join(result) + " One"
 
         class Transform2(FauxTransformBase):
-
             order = 1
 
             def transformUnicode(self, result, encoding):
-                return result.encode(encoding) + u' Two'.encode(encoding)
+                return result.encode(encoding) + " Two".encode(encoding)
 
         class Transform3(FauxTransformBase):
-
             order = 2
 
             def transformBytes(self, result, encoding):
-                return result.decode(encoding) + u' Three'
+                return result.decode(encoding) + " Three"
 
-        provideAdapter(Transform1, name=u'test.one')
-        provideAdapter(Transform2, name=u'test.two')
-        provideAdapter(Transform3, name=u'test.three')
+        provideAdapter(Transform1, name="test.one")
+        provideAdapter(Transform2, name="test.two")
+        provideAdapter(Transform3, name="test.three")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Blah']
-        encoding = 'utf-8'
+        result = ["Blah"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual(u'Blah One Two Three', new_result)
+        self.assertEqual("Blah One Two Three", new_result)
 
     def test_abort(self):
-
         class Transform1(FauxTransformBase):
             pass
 
-        provideAdapter(Transform1, name=u'test.one')
+        provideAdapter(Transform1, name="test.one")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Blah']
-        encoding = 'utf-8'
+        result = ["Blah"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual(['Blah'], new_result)
+        self.assertEqual(["Blah"], new_result)
 
     def test_abort_chain(self):
-
         class Transform1(FauxTransformBase):
-
             def transformBytes(self, result, encoding):
-                return b'One'
+                return b"One"
 
             def transformUnicode(self, result, encoding):
-                return u'One'
+                return "One"
 
             def transformIterable(self, result, encoding):
-                return 'One'
+                return "One"
 
         class Transform2(FauxTransformBase):
             pass
 
         class Transform3(FauxTransformBase):
-
             order = 2
 
             def transformBytes(self, result, encoding):
-                return result + b' three'
+                return result + b" three"
 
             def transformUnicode(self, result, encoding):
-                return result + u' three'
+                return result + " three"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' three'
+                return "".join(result) + " three"
 
-        provideAdapter(Transform1, name=u'test.one')
-        provideAdapter(Transform2, name=u'test.two')
-        provideAdapter(Transform3, name=u'test.three')
+        provideAdapter(Transform1, name="test.one")
+        provideAdapter(Transform2, name="test.two")
+        provideAdapter(Transform3, name="test.three")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Blah']
-        encoding = 'utf-8'
+        result = ["Blah"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('One three', new_result)
+        self.assertEqual("One three", new_result)
 
     def test_ordering(self):
-
         class Transform1(FauxTransformBase):
-
             order = 100
 
             def transformBytes(self, result, encoding):
-                return result + b' One'
+                return result + b" One"
 
             def transformUnicode(self, result, encoding):
-                return result + u' One'
+                return result + " One"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' One'
+                return "".join(result) + " One"
 
         class Transform2(FauxTransformBase):
-
             order = -100
 
             def transformBytes(self, result, encoding):
-                return result + b' Two'
+                return result + b" Two"
 
             def transformUnicode(self, result, encoding):
-                return result + u' Two'
+                return result + " Two"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' Two'
+                return "".join(result) + " Two"
 
         class Transform3(FauxTransformBase):
-
             order = 101
 
             def transformBytes(self, result, encoding):
-                return result + b' Three'
+                return result + b" Three"
 
             def transformUnicode(self, result, encoding):
-                return result + u' Three'
+                return result + " Three"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' Three'
+                return "".join(result) + " Three"
 
-        provideAdapter(Transform1, name=u'test.one')
-        provideAdapter(Transform2, name=u'test.two')
-        provideAdapter(Transform3, name=u'test.three')
+        provideAdapter(Transform1, name="test.one")
+        provideAdapter(Transform2, name="test.two")
+        provideAdapter(Transform3, name="test.three")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Initial']
-        encoding = 'utf-8'
+        result = ["Initial"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('Initial Two One Three', new_result)
+        self.assertEqual("Initial Two One Three", new_result)
 
     def test_request_marker(self):
-
         class Transform1(FauxTransformBase):
-
             order = 100
 
             def transformBytes(self, result, encoding):
-                return result + b' One'
+                return result + b" One"
 
             def transformUnicode(self, result, encoding):
-                return result + u' One'
+                return result + " One"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' One'
+                return "".join(result) + " One"
 
         class Transform2(FauxTransformBase):
-
             order = -100
 
             def transformBytes(self, result, encoding):
-                return result + b' Two'
+                return result + b" Two"
 
             def transformUnicode(self, result, encoding):
-                return result + u' Two'
+                return result + " Two"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' Two'
+                return "".join(result) + " Two"
 
         @implementer(ITransform)
         @adapter(Interface, IRequestMarker)
         class Transform3(FauxTransformBase):
-
             order = 101
 
             def transformBytes(self, result, encoding):
-                return result + b' Three'
+                return result + b" Three"
 
             def transformUnicode(self, result, encoding):
-                return result + u' Three'
+                return result + " Three"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' Three'
+                return "".join(result) + " Three"
 
-        provideAdapter(Transform1, name=u'test.one')
-        provideAdapter(Transform2, name=u'test.two')
-        provideAdapter(Transform3, name=u'test.three')
+        provideAdapter(Transform1, name="test.one")
+        provideAdapter(Transform2, name="test.two")
+        provideAdapter(Transform3, name="test.three")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Initial']
-        encoding = 'utf-8'
+        result = ["Initial"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('Initial Two One', new_result)
+        self.assertEqual("Initial Two One", new_result)
 
         published = FauxPublished()
         request = FauxRequest(published)
         alsoProvides(request, IRequestMarker)
-        result = ['Initial']
-        encoding = 'utf-8'
+        result = ["Initial"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('Initial Two One Three', new_result)
+        self.assertEqual("Initial Two One Three", new_result)
 
     def test_published_marker(self):
-
         class Transform1(FauxTransformBase):
-
             order = 100
 
             def transformBytes(self, result, encoding):
-                return result + b' One'
+                return result + b" One"
 
             def transformUnicode(self, result, encoding):
-                return result + u' One'
+                return result + " One"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' One'
+                return "".join(result) + " One"
 
         class Transform2(FauxTransformBase):
-
             order = -100
 
             def transformBytes(self, result, encoding):
-                return result + b' Two'
+                return result + b" Two"
 
             def transformUnicode(self, result, encoding):
-                return result + u' Two'
+                return result + " Two"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' Two'
+                return "".join(result) + " Two"
 
         @implementer(ITransform)
         @adapter(IPublishedMarker, Interface)
         class Transform3(FauxTransformBase):
-
             order = 101
 
             def transformBytes(self, result, encoding):
-                return result + b' Three'
+                return result + b" Three"
 
             def transformUnicode(self, result, encoding):
-                return result + u' Three'
+                return result + " Three"
 
             def transformIterable(self, result, encoding):
-                return ''.join(result) + ' Three'
+                return "".join(result) + " Three"
 
-        provideAdapter(Transform1, name=u'test.one')
-        provideAdapter(Transform2, name=u'test.two')
-        provideAdapter(Transform3, name=u'test.three')
+        provideAdapter(Transform1, name="test.one")
+        provideAdapter(Transform2, name="test.two")
+        provideAdapter(Transform3, name="test.three")
 
         published = FauxPublished()
         request = FauxRequest(published)
-        result = ['Initial']
-        encoding = 'utf-8'
+        result = ["Initial"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('Initial Two One', new_result)
+        self.assertEqual("Initial Two One", new_result)
 
         published = FauxPublished()
         alsoProvides(published, IPublishedMarker)
         request = FauxRequest(published)
-        result = ['Initial']
-        encoding = 'utf-8'
+        result = ["Initial"]
+        encoding = "utf-8"
 
         new_result = self.t(request, result, encoding)
-        self.assertEqual('Initial Two One Three', new_result)
+        self.assertEqual("Initial Two One Three", new_result)
 
 
 class TestZPublisherTransforms(unittest.TestCase):
-
     UNIT_TESTING
 
     def setUp(self):
         self.t = Transformer()
 
     def test_applyTransform_webdav_port(self):
-
         @implementer(ITransformer)
-        class DoNotCallTransformer(object):
+        class DoNotCallTransformer:
             encoding = None
 
             def __call__(self, request, result, encoding):
-                raise AssertionError('Should not have been called')
+                raise AssertionError("Should not have been called")
 
         transformer = DoNotCallTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request['WEBDAV_SOURCE_PORT'] = '8081'
+        request["WEBDAV_SOURCE_PORT"] = "8081"
         applyTransformOnSuccess(FauxPubEvent(request))
 
     def test_applyTransform_webdav_method(self):
         @implementer(ITransformer)
-        class DoNotCallTransformer(object):
+        class DoNotCallTransformer:
             encoding = None
 
             def __call__(self, request, result, encoding):
-                raise AssertionError('Should not have been called')
+                raise AssertionError("Should not have been called")
 
         transformer = DoNotCallTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request['REQUEST_METHOD'] = 'PUT'
+        request["REQUEST_METHOD"] = "PUT"
         applyTransformOnSuccess(FauxPubEvent(request))
 
     def test_applyTransform_webdav_pathinfo(self):
-
         @implementer(ITransformer)
-        class DoNotCallTransformer(object):
+        class DoNotCallTransformer:
             encoding = None
 
             def __call__(self, request, result, encoding):
-                raise AssertionError('Should not have been called')
+                raise AssertionError("Should not have been called")
 
         transformer = DoNotCallTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request['PATH_INFO'] = '/foo/bar/manage_DAVget'
+        request["PATH_INFO"] = "/foo/bar/manage_DAVget"
         applyTransformOnSuccess(FauxPubEvent(request))
 
     def test_applyTransform_no_utility(self):
         published = FauxPublished()
         request = FauxRequest(published)
         applyTransformOnSuccess(FauxPubEvent(request))
 
     def test_applyTransform_default_encoding(self):
-
         @implementer(ITransformer)
-        class EncodingCaptureTransformer(object):
+        class EncodingCaptureTransformer:
             encoding = None
 
             def __call__(self, request, result, encoding):
                 self.encoding = encoding
 
         transformer = EncodingCaptureTransformer()
         provideUtility(transformer)
@@ -561,160 +497,148 @@
         request = FauxRequest(published)
         applyTransformOnSuccess(FauxPubEvent(request))
 
         self.assertEqual(default_encoding, transformer.encoding)
 
     def test_applyTransform_other_encoding(self):
         @implementer(ITransformer)
-        class EncodingCaptureTransformer(object):
+        class EncodingCaptureTransformer:
             encoding = None
 
             def __call__(self, request, result, encoding):
                 self.encoding = encoding
 
         transformer = EncodingCaptureTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request.response.headers['content-type'] = 'text/html; charset=utf-16'
+        request.response.headers["content-type"] = "text/html; charset=utf-16"
         applyTransformOnSuccess(FauxPubEvent(request))
 
-        self.assertEqual('utf-16', transformer.encoding)
+        self.assertEqual("utf-16", transformer.encoding)
 
     def test_applyTransform_other_encoding_with_header_missing_space(self):
         @implementer(ITransformer)
-        class EncodingCaptureTransformer(object):
+        class EncodingCaptureTransformer:
             encoding = None
 
             def __call__(self, request, result, encoding):
                 self.encoding = encoding
 
         transformer = EncodingCaptureTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request.response.headers['content-type'] = 'text/html;charset=utf-16'
+        request.response.headers["content-type"] = "text/html;charset=utf-16"
         applyTransformOnSuccess(FauxPubEvent(request))
 
-        self.assertEqual('utf-16', transformer.encoding)
+        self.assertEqual("utf-16", transformer.encoding)
 
     def test_applyTransform_str(self):
         @implementer(ITransformer)
-        class FauxTransformer(object):
-
+        class FauxTransformer:
             def __call__(self, request, result, encoding):
-                return 'dummystr'
+                return "dummystr"
 
         transformer = FauxTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
         applyTransformOnSuccess(FauxPubEvent(request))
 
-        self.assertEqual('dummystr', request.response.getBody())
+        self.assertEqual("dummystr", request.response.getBody())
 
     def test_applyTransform_unicode(self):
         @implementer(ITransformer)
-        class FauxTransformer(object):
-
+        class FauxTransformer:
             def __call__(self, request, result, encoding):
-                return u'dummystr'
+                return "dummystr"
 
         transformer = FauxTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
         applyTransformOnSuccess(FauxPubEvent(request))
 
         # note: the real setBody would encode here
-        self.assertEqual(u'dummystr', request.response.getBody())
+        self.assertEqual("dummystr", request.response.getBody())
 
     def test_applyTransform_iterable(self):
         @implementer(ITransformer)
-        class FauxTransformer(object):
-
+        class FauxTransformer:
             def __call__(self, request, result, encoding):
-                return ['iter', 'one']
+                return ["iter", "one"]
 
         transformer = FauxTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
         applyTransformOnSuccess(FauxPubEvent(request))
 
-        self.assertEqual('iterone', request.response.getBody())
+        self.assertEqual("iterone", request.response.getBody())
 
     def test_applyTransform_streamiterator(self):
         tmp = tempfile.mkstemp()[1]
         try:
-
-            with open(tmp, 'w') as out:
-                out.write('foo')
+            with open(tmp, "w") as out:
+                out.write("foo")
 
             @implementer(ITransformer)
-            class FauxTransformer(object):
-
+            class FauxTransformer:
                 def __call__(self, request, result, encoding):
                     return filestream_iterator(tmp)
 
             transformer = FauxTransformer()
             provideUtility(transformer)
 
             published = FauxPublished()
             request = FauxRequest(published)
             applyTransformOnSuccess(FauxPubEvent(request))
 
-            self.assertTrue(
-                isinstance(
-                    request.response.getBody(),
-                    filestream_iterator
-                )
-            )
+            self.assertTrue(isinstance(request.response.getBody(), filestream_iterator))
         finally:
             os.unlink(tmp)
 
     def test_applyTransform_str_input_body(self):
         @implementer(ITransformer)
-        class FauxTransformer(object):
-
+        class FauxTransformer:
             def __call__(self, request, result, encoding):
                 assert isinstance(result, list)
-                assert isinstance(result[0], six.binary_type)
-                return 'dummystr'
+                assert isinstance(result[0], bytes)
+                return "dummystr"
 
         transformer = FauxTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request.response.setBody('<html />')
+        request.response.setBody("<html />")
 
         applyTransformOnSuccess(FauxPubEvent(request))
 
         # note: the real setBody would encode here
-        self.assertEqual('dummystr', request.response.getBody())
+        self.assertEqual("dummystr", request.response.getBody())
 
     def test_applyTransform_unicode_input_body(self):
         @implementer(ITransformer)
-        class FauxTransformer(object):
-
+        class FauxTransformer:
             def __call__(self, request, result, encoding):
                 assert isinstance(result, list)
-                assert isinstance(result[0], six.binary_type)
-                return u'dummystr'
+                assert isinstance(result[0], bytes)
+                return "dummystr"
 
         transformer = FauxTransformer()
         provideUtility(transformer)
 
         published = FauxPublished()
         request = FauxRequest(published)
-        request.response.setBody(u'<html />')
+        request.response.setBody("<html />")
 
         applyTransformOnSuccess(FauxPubEvent(request))
 
         # note: the real setBody would encode here
-        self.assertEqual(u'dummystr', request.response.getBody())
+        self.assertEqual("dummystr", request.response.getBody())
```

### Comparing `plone.transformchain-2.0.2/plone.transformchain.egg-info/SOURCES.txt` & `plone.transformchain-3.0.0/plone.transformchain.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 setup.cfg
 setup.py
 docs/INSTALL.txt
 plone/__init__.py
 plone.transformchain.egg-info/PKG-INFO
 plone.transformchain.egg-info/SOURCES.txt
 plone.transformchain.egg-info/dependency_links.txt
-plone.transformchain.egg-info/entry_points.txt
 plone.transformchain.egg-info/namespace_packages.txt
 plone.transformchain.egg-info/not-zip-safe
 plone.transformchain.egg-info/requires.txt
 plone.transformchain.egg-info/top_level.txt
 plone/transformchain/__init__.py
 plone/transformchain/configure.zcml
 plone/transformchain/events.py
```

### Comparing `plone.transformchain-2.0.2/README.rst` & `plone.transformchain-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.transformchain-2.0.2/CHANGES.rst` & `plone.transformchain-3.0.0/CHANGES.rst`

 * *Files 6% similar despite different names*

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
+- Drop Python 2 and Plone 5.2 compatibility.
+  [gforcada] (#6)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (3333c742)
+
+
 2.0.2 (2020-04-22)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
```

