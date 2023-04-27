# Comparing `tmp/pysnc-1.1.2.tar.gz` & `tmp/pysnc-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.2.tar", max compression
+gzip compressed data, was "pysnc-1.1.3.tar", max compression
```

## Comparing `pysnc-1.1.2.tar` & `pysnc-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-04-26 23:06:05.738981 pysnc-1.1.2/LICENSE
--rw-r--r--   0        0        0     1590 2023-04-26 23:06:05.738981 pysnc-1.1.2/README.md
--rw-r--r--   0        0        0      984 2023-04-26 23:06:05.742981 pysnc-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/__version__.py
--rw-r--r--   0        0        0     8875 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/attachment.py
--rw-r--r--   0        0        0     3778 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/auth.py
--rw-r--r--   0        0        0    15569 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/client.py
--rw-r--r--   0        0        0     1002 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/exceptions.py
--rw-r--r--   0        0        0     3809 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/query.py
--rw-r--r--   0        0        0    37242 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-04-26 23:06:05.742981 pysnc-1.1.2/pysnc/utils.py
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-04-27 21:10:59.586770 pysnc-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1590 2023-04-27 21:10:59.586770 pysnc-1.1.3/README.md
+-rw-r--r--   0        0        0      984 2023-04-27 21:10:59.586770 pysnc-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-04-27 21:10:59.586770 pysnc-1.1.3/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-27 21:10:59.586770 pysnc-1.1.3/pysnc/__version__.py
+-rw-r--r--   0        0        0     8875 2023-04-27 21:10:59.586770 pysnc-1.1.3/pysnc/attachment.py
+-rw-r--r--   0        0        0     3778 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/auth.py
+-rw-r--r--   0        0        0    15712 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3809 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/query.py
+-rw-r--r--   0        0        0    37242 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-04-27 21:10:59.590770 pysnc-1.1.3/pysnc/utils.py
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 pysnc-1.1.3/PKG-INFO
```

### Comparing `pysnc-1.1.2/LICENSE` & `pysnc-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/README.md` & `pysnc-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/pyproject.toml` & `pysnc-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.2"
+version = "1.1.3"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
```

### Comparing `pysnc-1.1.2/pysnc/attachment.py` & `pysnc-1.1.3/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/pysnc/auth.py` & `pysnc-1.1.3/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/pysnc/client.py` & `pysnc-1.1.3/pysnc/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,15 +170,17 @@
                         self.session.refresh_token(self.session.auto_refresh_url)
                     else:
                         raise e
                 else:
                     raise e
 
         request = self.session.prepare_request(req)
-        r = self.session.send(request, stream=stream)
+        # Merge environment settings into session
+        settings = self.session.merge_environment_settings(request.url, {}, stream, None, None)
+        r = self.session.send(request, **settings)
         self._validate_response(r)
         return r
 
 
 class TableAPI(API):
 
     def _target(self, table, sys_id=None) -> str:
```

### Comparing `pysnc-1.1.2/pysnc/exceptions.py` & `pysnc-1.1.3/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/pysnc/query.py` & `pysnc-1.1.3/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/pysnc/record.py` & `pysnc-1.1.3/pysnc/record.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/pysnc/utils.py` & `pysnc-1.1.3/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.2/PKG-INFO` & `pysnc-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
```

