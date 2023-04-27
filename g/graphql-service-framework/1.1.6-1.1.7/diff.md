# Comparing `tmp/graphql_service_framework-1.1.6.tar.gz` & `tmp/graphql_service_framework-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.1.6.tar", last modified: Thu Apr 27 13:40:32 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.7.tar", last modified: Thu Apr 27 15:34:18 2023, max compression
```

## Comparing `graphql_service_framework-1.1.6.tar` & `graphql_service_framework-1.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:40:32.740493 graphql_service_framework-1.1.6/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 13:40:32.741493 graphql_service_framework-1.1.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-27 13:40:32.000000 graphql_service_framework-1.1.6/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:40:32.737492 graphql_service_framework-1.1.6/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15660 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/query.graphql
--rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7738 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/service.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/graphql_service_framework/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:40:32.739493 graphql_service_framework-1.1.6/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 13:40:32.000000 graphql_service_framework-1.1.6/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-27 13:40:32.000000 graphql_service_framework-1.1.6/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 13:40:32.000000 graphql_service_framework-1.1.6/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-27 13:40:32.000000 graphql_service_framework-1.1.6/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-27 13:40:32.000000 graphql_service_framework-1.1.6/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-27 13:40:32.741493 graphql_service_framework-1.1.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 13:40:32.740493 graphql_service_framework-1.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/tests/test_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-27 13:40:21.000000 graphql_service_framework-1.1.6/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:18.156663 graphql_service_framework-1.1.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 15:34:18.156663 graphql_service_framework-1.1.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-27 15:34:17.000000 graphql_service_framework-1.1.7/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:18.153913 graphql_service_framework-1.1.7/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15660 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/query.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7619 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:18.154830 graphql_service_framework-1.1.7/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 15:34:18.000000 graphql_service_framework-1.1.7/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-27 15:34:18.000000 graphql_service_framework-1.1.7/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 15:34:18.000000 graphql_service_framework-1.1.7/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-27 15:34:18.000000 graphql_service_framework-1.1.7/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-27 15:34:18.000000 graphql_service_framework-1.1.7/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-27 15:34:18.157580 graphql_service_framework-1.1.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:18.156663 graphql_service_framework-1.1.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-27 15:34:08.000000 graphql_service_framework-1.1.7/tests/utils.py
```

### Comparing `graphql_service_framework-1.1.6/LICENSE` & `graphql_service_framework-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/PKG-INFO` & `graphql_service_framework-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.1.6
+Version: 1.1.7
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.6.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.7.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/conftest.py` & `graphql_service_framework-1.1.7/graphql_service_framework/conftest.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/mesh.py` & `graphql_service_framework-1.1.7/graphql_service_framework/mesh.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/middleware.py` & `graphql_service_framework-1.1.7/graphql_service_framework/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.7/graphql_service_framework/schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.7/graphql_service_framework/schema_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,35 +72,32 @@
 
     def __hash__(self):
         return hash((self.name, self.path))
 
     @functools.cache
     def previous_schema(self) -> Optional[Type[Schema]]:
         # noinspection PyBroadException
-        try:
-            print(f"Checking for a previous version of {self.name}")
-            _prev_report = install_package(self.name, index_url=self.index_url)
-
-            if _prev_report:
-                v = _prev_report["install"][0]["metadata"]["version"]
-
-                install_location = _prev_report.get("pip_show").get("Location")
-                print(
-                    f"Installed package " f"{self.name} version {v} at "
-                    f"{install_location}"
-                )
-
-                prev_modules = find_modules(
-                    os.path.join(install_location, self.package_name, self.name),
-                    f"{self.package_name}.{self.name}",
-                )
-
-                return find_schema(prev_modules)
-        except Exception:
-            return None
+        print(f"Checking for a previous version of {self.name}")
+        _prev_report = install_package(self.name, index_url=self.index_url)
+
+        if _prev_report:
+            v = _prev_report["install"][0]["metadata"]["version"]
+
+            install_location = _prev_report.get("pip_show").get("Location")
+            print(
+                f"Installed package " f"{self.name} version {v} at "
+                f"{install_location}"
+            )
+
+            prev_modules = find_modules(
+                os.path.join(install_location, self.package_name, self.name),
+                f"{self.package_name}.{self.name}",
+            )
+
+            return find_schema(prev_modules)
 
     @functools.cache
     def code_changes(self):
         if self.previous_schema():
             a_path = self.path
             b_path = os.path.dirname(
                 importlib.import_module(f"{self.package_name}.{self.name}").__file__
```

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/service.py` & `graphql_service_framework-1.1.7/graphql_service_framework/service.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.7/graphql_service_framework/utils.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.7/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.1.6
+Version: 1.1.7
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.6.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.7.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.6/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.7/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/setup.py` & `graphql_service_framework-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/tests/test_schema.py` & `graphql_service_framework-1.1.7/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/tests/test_service_manager.py` & `graphql_service_framework-1.1.7/tests/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.6/tests/utils.py` & `graphql_service_framework-1.1.7/tests/utils.py`

 * *Files identical despite different names*

