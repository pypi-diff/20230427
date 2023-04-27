# Comparing `tmp/graphql_service_framework-1.1.3.tar.gz` & `tmp/graphql_service_framework-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.1.3.tar", last modified: Tue Apr 25 19:07:58 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.4.tar", last modified: Wed Apr 26 17:15:12 2023, max compression
```

## Comparing `graphql_service_framework-1.1.3.tar` & `graphql_service_framework-1.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.584151 graphql_service_framework-1.1.3/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-25 19:07:58.585151 graphql_service_framework-1.1.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-25 19:07:57.000000 graphql_service_framework-1.1.3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.581151 graphql_service_framework-1.1.3/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15650 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/query.graphql
--rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     5303 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/service.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/graphql_service_framework/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.583151 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-25 19:07:58.000000 graphql_service_framework-1.1.3/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-25 19:07:58.585151 graphql_service_framework-1.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 19:07:58.584151 graphql_service_framework-1.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/test_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-25 19:07:48.000000 graphql_service_framework-1.1.3/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:15:12.910590 graphql_service_framework-1.1.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-26 17:15:12.910590 graphql_service_framework-1.1.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-26 17:15:12.000000 graphql_service_framework-1.1.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:15:12.907589 graphql_service_framework-1.1.4/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15660 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/query.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:15:12.909589 graphql_service_framework-1.1.4/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-26 17:15:12.000000 graphql_service_framework-1.1.4/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-26 17:15:12.000000 graphql_service_framework-1.1.4/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 17:15:12.000000 graphql_service_framework-1.1.4/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-26 17:15:12.000000 graphql_service_framework-1.1.4/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-26 17:15:12.000000 graphql_service_framework-1.1.4/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-26 17:15:12.911590 graphql_service_framework-1.1.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 17:15:12.910590 graphql_service_framework-1.1.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-26 17:15:03.000000 graphql_service_framework-1.1.4/tests/utils.py
```

### Comparing `graphql_service_framework-1.1.3/LICENSE` & `graphql_service_framework-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/PKG-INFO` & `graphql_service_framework-1.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.1.3
+Version: 1.1.4
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.3.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.4.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/conftest.py` & `graphql_service_framework-1.1.4/graphql_service_framework/conftest.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/mesh.py` & `graphql_service_framework-1.1.4/graphql_service_framework/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
         return self.__getattr__(item)
 
     @field
     def name(self) -> str:
         return self._name
 
     @field
-    def api_version(self) -> str:
+    def api_version(self) -> Optional[str]:
         return self._api_version
 
     @field
     def service_version(self) -> str:
         return self._service_version
 
     @field
```

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/middleware.py` & `graphql_service_framework-1.1.4/graphql_service_framework/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.4/graphql_service_framework/schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.4/graphql_service_framework/schema_tracker.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/service.py` & `graphql_service_framework-1.1.4/graphql_service_framework/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,35 +39,36 @@
 
         if not self.config.get("http_health_path"):
             self.config["http_health_path"] = f"{relative_path}/health"
 
         health_path = self.config.get("http_health_path")
 
         if not graphiql_default:
-            # noinspection PyBroadException
-            try:
-                dirname = os.path.dirname(inspect.getfile(root.__class__))
-                graphiql_default = open(
-                    os.path.join(dirname, "../graphiql_default.graphql"), mode="r"
-                ).read()
-            except Exception:
-                # noinspection PyBroadException
-                try:
-                    dirname = os.path.dirname(inspect.getfile(root.__class__))
-                    graphiql_default = open(
-                        os.path.join(dirname, "../.graphql"), mode="r"
-                    ).read()
-                except Exception:
-                    try:
-                        dirname = os.path.dirname(inspect.getfile(root.__class__))
-                        graphiql_default = open(
-                            os.path.join(dirname, "./.graphql"), mode="r"
-                        ).read()
-                    except Exception:
-                        pass
+            dirs = [
+                os.path.dirname(inspect.getfile(root.__class__)),
+                os.getcwd()
+            ]
+            file_names = [
+                "./.graphql",
+                "../.graphql",
+            ]
+
+            for _dir in dirs:
+                if not graphiql_default:
+                    for _file_name in file_names:
+                        # noinspection PyBroadException
+                        try:
+                            graphiql_default = open(
+                                os.path.join(_dir, _file_name),
+                                mode="r"
+                            ).read()
+                            break
+                        # noinspection PyBroadException
+                        except Exception:
+                            pass
 
         self.graphql_api = GraphQLAPI(root=root.__class__)
         self.graphql_http_server = GraphQLHTTPServer.from_api(
             api=self.graphql_api,
             root_value=root,
             graphiql_default_query=graphiql_default,
             health_path=health_path,
```

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.4/graphql_service_framework/utils.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.4/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.1.3
+Version: 1.1.4
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.3.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.4.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.3/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.4/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/setup.py` & `graphql_service_framework-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/tests/test_schema.py` & `graphql_service_framework-1.1.4/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/tests/test_service_manager.py` & `graphql_service_framework-1.1.4/tests/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.3/tests/utils.py` & `graphql_service_framework-1.1.4/tests/utils.py`

 * *Files identical despite different names*

