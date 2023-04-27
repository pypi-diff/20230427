# Comparing `tmp/mlx.coverity-1.0.0.tar.gz` & `tmp/mlx.coverity-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx.coverity-1.0.0.tar", last modified: Mon Mar  6 09:52:52 2023, max compression
+gzip compressed data, was "mlx.coverity-1.0.1.tar", last modified: Thu Apr 27 08:40:47 2023, max compression
```

## Comparing `mlx.coverity-1.0.0.tar` & `mlx.coverity-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.116405 mlx.coverity-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/.codeclimate.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-03-06 09:52:52.116405 mlx.coverity-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/example/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/example/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/example/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-03-06 09:52:31.000000 mlx.coverity-1.0.0/example/_build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/example/_build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-03-06 09:52:32.000000 mlx.coverity-1.0.0/example/_build/html/_static/css/badge_only.css
--rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-03-06 09:52:32.000000 mlx.coverity-1.0.0/example/_build/html/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-06 09:52:31.000000 mlx.coverity-1.0.0/example/_build/html/_static/graphviz.css
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-06 09:52:31.000000 mlx.coverity-1.0.0/example/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-06 09:52:31.000000 mlx.coverity-1.0.0/example/_build/html/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/example/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/example/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.112405 mlx.coverity-1.0.0/mlx/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/coverity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.116405 mlx.coverity-1.0.0/mlx/coverity_directives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/coverity_directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/coverity_directives/coverity_defect_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/coverity_item_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/coverity_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/mlx/coverity_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.116405 mlx.coverity-1.0.0/mlx.coverity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-03-06 09:52:51.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-06 09:52:52.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:52:51.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 09:52:51.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:52:51.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-06 09:52:51.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 09:52:51.000000 mlx.coverity-1.0.0/mlx.coverity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-06 09:52:52.116405 mlx.coverity-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:52.116405 mlx.coverity-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/tests/defect_soap.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/tests/test_coverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-06 09:52:30.000000 mlx.coverity-1.0.0/warnings_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.728499 mlx.coverity-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/.codeclimate.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.720499 mlx.coverity-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.724499 mlx.coverity-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-04-27 08:40:47.728499 mlx.coverity-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.720499 mlx.coverity-1.0.1/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.720499 mlx.coverity-1.0.1/example/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.720499 mlx.coverity-1.0.1/example/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.724499 mlx.coverity-1.0.1/example/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-04-27 08:40:07.000000 mlx.coverity-1.0.1/example/_build/html/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.724499 mlx.coverity-1.0.1/example/_build/html/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-27 08:40:07.000000 mlx.coverity-1.0.1/example/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-04-27 08:40:07.000000 mlx.coverity-1.0.1/example/_build/html/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 08:40:07.000000 mlx.coverity-1.0.1/example/_build/html/_static/graphviz.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-27 08:40:07.000000 mlx.coverity-1.0.1/example/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-27 08:40:07.000000 mlx.coverity-1.0.1/example/_build/html/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.724499 mlx.coverity-1.0.1/example/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/example/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.724499 mlx.coverity-1.0.1/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/coverity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.728499 mlx.coverity-1.0.1/mlx/coverity_directives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/coverity_directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/coverity_directives/coverity_defect_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/coverity_item_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/coverity_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25382 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/mlx/coverity_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.728499 mlx.coverity-1.0.1/mlx.coverity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 08:40:47.000000 mlx.coverity-1.0.1/mlx.coverity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 08:40:47.728499 mlx.coverity-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:47.728499 mlx.coverity-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/tests/defect_soap.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/tests/test_coverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-27 08:40:06.000000 mlx.coverity-1.0.1/warnings_config.json
```

### Comparing `mlx.coverity-1.0.0/.codeclimate.yml` & `mlx.coverity-1.0.1/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/.github/workflows/python-package.yml` & `mlx.coverity-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/LICENSE` & `mlx.coverity-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/MANIFEST.in` & `mlx.coverity-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/PKG-INFO` & `mlx.coverity-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.coverity
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sphinx coverity extension from Melexis
 Home-page: https://github.com/melexis/sphinx-coverity-extension
 Author: Crt Mori
 Author-email: cmo@melexis.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: coverity,reporting,reStructuredText coverity report,sphinx,ASPICE,ISO26262,ASIL
 Platform: any
```

### Comparing `mlx.coverity-1.0.0/README.rst` & `mlx.coverity-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/example/_build/html/_static/basic.css` & `mlx.coverity-1.0.1/example/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/example/_build/html/_static/css/badge_only.css` & `mlx.coverity-1.0.1/example/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/example/_build/html/_static/css/theme.css` & `mlx.coverity-1.0.1/example/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/example/_build/html/_static/pygments.css` & `mlx.coverity-1.0.1/example/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/mlx/coverity.py` & `mlx.coverity-1.0.1/mlx/coverity.py`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/mlx/coverity_directives/coverity_defect_list.py` & `mlx.coverity-1.0.1/mlx/coverity_directives/coverity_defect_list.py`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/mlx/coverity_item_element.py` & `mlx.coverity-1.0.1/mlx/coverity_item_element.py`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/mlx/coverity_logging.py` & `mlx.coverity-1.0.1/mlx/coverity_logging.py`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/mlx/coverity_services.py` & `mlx.coverity-1.0.1/mlx/coverity_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,18 +110,18 @@
         '''Set WS version for service'''
         self.ws_version = ws_version
 
     def get_ws_version(self):
         '''Get WS version for service'''
         return self.ws_version
 
-    def get_service_url(self, path=''):
+    def get_service_url(self, path='', add_port=True):
         '''Get Service url with given path'''
         url = self.transport + '://' + self.hostname
-        if bool(self.port):
+        if self.port and add_port:
             url += ':' + self.port
         if path:
             url += path
         return url
 
     def get_ws_url(self, service):
         '''Get WS url with given service'''
@@ -601,14 +601,14 @@
 
     def get_action(self, stream_defect):
         '''Get action attribute value for given defect'''
         return self.get_value_for_named_attribute(stream_defect, ACTION_ATTR_NAME)
 
     def get_defect_url(self, stream, cid):
         '''Get URL for given defect CID
-        http://machine1.eng.company.com:8080/query/defects.htm?stream=StreamA&cid=1234
+        http://machine1.eng.company.com/query/defects.htm?stream=StreamA&cid=1234
         '''
-        return self.get_service_url('/query/defects.htm?stream=%s&cid=%s' % (stream, str(cid)))
+        return self.get_service_url('/query/defects.htm?stream=%s&cid=%s' % (stream, str(cid)), add_port=False)
 
 
 if __name__ == '__main__':
     print("Sorry, no main here")
```

### Comparing `mlx.coverity-1.0.0/mlx.coverity.egg-info/PKG-INFO` & `mlx.coverity-1.0.1/mlx.coverity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.coverity
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sphinx coverity extension from Melexis
 Home-page: https://github.com/melexis/sphinx-coverity-extension
 Author: Crt Mori
 Author-email: cmo@melexis.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: coverity,reporting,reStructuredText coverity report,sphinx,ASPICE,ISO26262,ASIL
 Platform: any
```

### Comparing `mlx.coverity-1.0.0/mlx.coverity.egg-info/SOURCES.txt` & `mlx.coverity-1.0.1/mlx.coverity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/setup.py` & `mlx.coverity-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/tests/defect_soap.xml` & `mlx.coverity-1.0.1/tests/defect_soap.xml`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/tests/test_coverity.py` & `mlx.coverity-1.0.1/tests/test_coverity.py`

 * *Files identical despite different names*

### Comparing `mlx.coverity-1.0.0/tox.ini` & `mlx.coverity-1.0.1/tox.ini`

 * *Files identical despite different names*

