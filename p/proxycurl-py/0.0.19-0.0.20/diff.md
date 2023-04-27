# Comparing `tmp/proxycurl-py-0.0.19.tar.gz` & `tmp/proxycurl-py-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxycurl-py-0.0.19.tar", last modified: Thu Apr 27 05:48:53 2023, max compression
+gzip compressed data, was "proxycurl-py-0.0.20.tar", last modified: Thu Apr 27 06:07:33 2023, max compression
```

## Comparing `proxycurl-py-0.0.19.tar` & `proxycurl-py-0.0.20.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/PKG-INFO
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12288 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/README.md
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/asyncio/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/asyncio/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4709 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/asyncio/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    72492 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/asyncio/library.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      283 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/config.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/gevent/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/gevent/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4171 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/gevent/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70856 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/gevent/library.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    14796 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/models.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/twisted/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/twisted/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4995 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/twisted/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70542 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/twisted/library.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py.egg-info/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/PKG-INFO
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      583 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/SOURCES.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)        1 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/dependency_links.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      168 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/requires.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       13 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/top_level.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      772 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/pyproject.toml
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       38 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/setup.cfg
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      985 2023-04-27 05:48:42.000000 proxycurl-py-0.0.19/setup.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/tests/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       80 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/tests/test_proxycurl.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/PKG-INFO
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12288 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/README.md
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.848605 proxycurl-py-0.0.20/proxycurl_py/
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py/asyncio/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/asyncio/__init__.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4709 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/asyncio/base.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    72492 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/asyncio/library.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      283 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/config.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py/gevent/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/gevent/__init__.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4171 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/gevent/base.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70856 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/gevent/library.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    14796 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/models.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py/twisted/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/twisted/__init__.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4995 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/twisted/base.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70542 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/twisted/library.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py.egg-info/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/PKG-INFO
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      583 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)        1 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      168 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/requires.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       13 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/top_level.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      772 2023-04-27 06:06:45.000000 proxycurl-py-0.0.20/pyproject.toml
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       38 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/setup.cfg
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      985 2023-04-27 06:06:52.000000 proxycurl-py-0.0.20/setup.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/tests/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       80 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/tests/test_proxycurl.py
```

### Comparing `proxycurl-py-0.0.19/PKG-INFO` & `proxycurl-py-0.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxycurl-py
-Version: 0.0.19
+Version: 0.0.20
 Author: Nubela
 Author-email: tech@nubela.co
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: gevent
 Provides-Extra: twisted
```

### Comparing `proxycurl-py-0.0.19/README.md` & `proxycurl-py-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/asyncio/base.py` & `proxycurl-py-0.0.20/proxycurl_py/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/asyncio/library.py` & `proxycurl-py-0.0.20/proxycurl_py/asyncio/library.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/gevent/base.py` & `proxycurl-py-0.0.20/proxycurl_py/gevent/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/gevent/library.py` & `proxycurl-py-0.0.20/proxycurl_py/gevent/library.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/models.py` & `proxycurl-py-0.0.20/proxycurl_py/models.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/twisted/base.py` & `proxycurl-py-0.0.20/proxycurl_py/twisted/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py/twisted/library.py` & `proxycurl-py-0.0.20/proxycurl_py/twisted/library.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/proxycurl_py.egg-info/PKG-INFO` & `proxycurl-py-0.0.20/proxycurl_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxycurl-py
-Version: 0.0.19
+Version: 0.0.20
 Author: Nubela
 Author-email: tech@nubela.co
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: gevent
 Provides-Extra: twisted
```

### Comparing `proxycurl-py-0.0.19/proxycurl_py.egg-info/SOURCES.txt` & `proxycurl-py-0.0.20/proxycurl_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.19/pyproject.toml` & `proxycurl-py-0.0.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proxycurl_py"
-version = "0.0.18"
+version = "0.0.20"
 description = ""
 readme = "README.md"
 authors = ["Nubela <tech@nubela.co>"]
 packages = [
     { include = "proxycurl_py"}
 ]
```

### Comparing `proxycurl-py-0.0.19/setup.py` & `proxycurl-py-0.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = \
 {'asyncio': ['asyncio>=3.4.3,<4.0.0', 'aiohttp>=3.7.4,<4.0.0'],
  'gevent': ['gevent>=21.1.1,<22.0.0', 'requests>=2.25.0,<3.0.0'],
  'twisted': ['Twisted>=21.7.0,<22.0.0', 'treq>=21.5.0,<22.0.0']}
 
 setup_kwargs = {
     'name': 'proxycurl-py',
-    'version': '0.0.19',
+    'version': '0.0.20',
     'description': '',
     'long_description_content_type':"text/markdown",
     'long_description': long_description,
     'author': 'Nubela',
     'author_email': 'tech@nubela.co',
     'maintainer': None,
     'maintainer_email': None,
```

